# FileMaker AI Vocabulary

[![License](https://img.shields.io/badge/license-CC%20BY%204.0-green)](https://creativecommons.org/licenses/by/4.0/)

**Every FileMaker 26 function and script step, in about 7,000 tokens.**

Small enough to load into context as part of the skill, so the model has the whole vocabulary in front of it while it writes, instead of guessing from training data and inventing functions that don't exist. The raw Claris help pages for the functions alone run to roughly 122,000 tokens. This is the same knowledge at roughly 1/30th the token footprint.

Developed by Andrew Kear of Clockwork Creative Technology and shared openly with the FileMaker/Claris community.

## The problem it solves

FileMaker's namespace is large and full of near-identical names: `Right`, `RightWords`, `RightValues`; `GetField`, `GetFieldName`. An AI generating a calculation guesses from training data and confidently invents a function that sounds right, or transposes a parameter, or assumes the wrong return type. The fix is to hand it the real vocabulary as ground truth, but a reference only helps if it's loaded at the moment of generation, not fetched afterward. Most references are too big to keep resident. This one isn't. That's the whole idea.

## What's inside

Two flat files, one line per entry, no prose to wade through:

- **368 functions** — exact name, parameter order, optional-parameter shape, return type.
- **216 script steps** — exact name, internal ID, and platform support across all seven FileMaker clients and hosts.

```
Case ( test1 ; result1 {; test2 ; result2 ; ... ; defaultResult} ) → text, number, date, time, timestamp, container
Substitute ( text ; [search1 ; replace1] {; [search2 ; replace2] ; ...} ) → text
Set Variable   #141
Perform Script On Server   #164   ⚠ Go:No, WebD:No
```

Return types are carried because models infer them wrongly when chaining calculations, not just function names. It's a constrained vocabulary, not a manual: enough to verify a name, a signature, and where a step runs, and nothing to slow the model down getting there.

## Deliberately just the vocabulary

This file answers the cheap, always-loaded questions: does this exist, what's it called, what are its parameters, where does it run. It does **not** carry a step's full option structure or paste-ready XML. That depth lives in the companion [Script XML Skill](https://github.com/andykear/FileMaker-XMLsnippet-Claude-Skill), and keeping it there is the point: the vocabulary layer stays tiny enough to stay resident, the generation layer holds the detail. Two layers, on purpose.

The step IDs here are pinned to that skill, so an ID in this file is the same ID it emits. They cannot drift.

## Target: FileMaker 26

A decision, not an oversight. Anyone pairing FileMaker with agentic AI is running current, and dropping version tags is part of what keeps the files this small.

## Use it

Load the release zip into Claude's skills (keep the folder structure; enable code execution and file creation). With the skill enabled, Claude consults the vocabulary when writing or reviewing FileMaker calculations and scripts, no special prompt. Setup varies by platform, so follow Anthropic's current instructions for adding a skill.

Model-agnostic by design: the files are plain markdown, readable by any LLM or human. Building your own FileMaker tooling? They're yours to integrate.

```
"Write a calc that strips the domain off an email address"
"Write a server-scheduled script to find overdue invoices"   → steps checked against platform support first
"Does FileMaker have a JSONMerge function?"                   → answered no, pointed to the real one
```

## The FileMaker XML suite

The companion to a set of skills and tools that reverse-engineer FileMaker's undocumented clipboard formats. Those decode formats Claris has never published; this compresses the formats Claris *does* document into the smallest resident form. Different work, same goal: AI that generates FileMaker that actually works.

**[Script XML Skill](https://github.com/andykear/FileMaker-XMLsnippet-Claude-Skill)** (XMSS, XMSC, XMFN) — the full script step ID dictionary and the hidden paste-handler rules that decide whether your XML survives the trip into FileMaker. This vocabulary's IDs are cross-referenced from it.

**[Layout XML Skill](https://github.com/andykear/FileMaker-XMLsnippet-Layout-Claude-Skill)** (XML2) — all 18 layout object types mapped, every flag decoded, element order confirmed against native output. Verified across 45+ layouts in 10 production files.

**[Field, Table & Value List Definitions](https://github.com/andykear/FileMaker-XML-field-definitions)** (XMFD, XMTB, XMVL) — schema definition XML, verified down to the individual option level.

**[XML Inspector](https://github.com/andykear/FileMaker-XML-inspector-open-source)** (SaXML) — full-catalog dependency analysis of a Save as XML export, in the browser. Finds unreferenced objects, silent-failure risks, broken references, and diffs two solution versions.

**[XML Scrubber](https://github.com/andykear/FileMaker-XML-scrubber)** — strips API keys, passwords and internal hostnames out of FileMaker XML before you hand it to an AI tool.

## Provenance

Function signatures, return types, and platform support come from [Claris FileMaker Pro Help](https://help.claris.com/en/pro-help/) — Claris's published facts, compression the only transformation. The verified internal step IDs come from the Clockwork Script XML skill; Claris doesn't publish them, they're original reverse-engineering work. If republishing, credit Claris for the function and compatibility data and the Clockwork FileMaker XML skills for the step IDs.

## Licence & contributing

CC BY 4.0 — free to use, share, and adapt with attribution. Found something missing, misnamed, or wrong on a return type or compatibility flag? Open an issue or PR.

## Version history

| Version | Notes |
|---|---|
| 1.0 | FileMaker 26 baseline. 368 functions (371 signature lines; `Substitute`, `JSONSetElement`, and `ComputeModel` carry a second signature recovered from description prose the Format field omits). 216 script steps with platform support, each carrying its verified internal ID from the Script XML skill. ~7,000 tokens total. |

---

*Clockwork Creative Technology — clockworkct.co.uk · github.com/andykear. Bespoke FileMaker development, automated artwork systems, and hosted solutions. Working on something and need a hand? Get in touch.*
