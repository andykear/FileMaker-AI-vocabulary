```text
# FileMaker Pro script step index, compressed. Target: FileMaker 26.
# This is the authoritative list of every script step that exists. Rules:
# - Only use script steps that appear below. Never invent a step. If a plausible-sounding step is not listed, it does not exist — say so.
# - The name shown is the exact canonical step name.
# - #NN is the step's internal ID, cross-referenced from the verified FileMaker Script XML paste skill.
# - This index does NOT list step options. For option names, element structure, and paste-ready XML, the FileMaker Script XML and Field XML skills are authoritative — defer to them rather than guessing options from this file.
# - ⚠ marks platforms where the step is No (unsupported) or Partial (works differently). No ⚠ means Yes everywhere: Pro, Go, WebDirect, Server, Cloud, Data API, Custom Web Publishing.

# (Comment)   #89
Add Account   #134
Adjust Window   #31   ⚠ Go:Partial, WebD:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Allow Formatting Bar   #115   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Allow User Abort   #85   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Append PDF   #244   ⚠ WebD:Partial
Arrange All Windows   #120   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
AVPlayer Play   #177   ⚠ Pro:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
AVPlayer Set Options   #179   ⚠ Pro:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
AVPlayer Set Playback State   #178   ⚠ Pro:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Beep   #93   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Cancel PDF   #247
Change Password   #83   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Check Found Set   #20   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Check Record   #19   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Check Selection   #18   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:Partial, CWP:Partial
Clear   #49   ⚠ WebD:Partial
Close Data File   #196   ⚠ WebD:No, DataAPI:No
Close File   #34   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Close PDF   #245   ⚠ WebD:Partial
Close Popover   #169   ⚠ Server:No, Cloud:No, DataAPI:No, CWP:No
Close Window   #121
Commit Records/Requests   #75   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Commit Transaction   #206
Configure AI Account   #212
Configure Local Notification   #187   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Configure Machine Learning Model   #202   ⚠ Pro:Partial, WebD:No, Server:Partial, Cloud:No, DataAPI:No, CWP:No
Configure NFC Reading   #201   ⚠ Pro:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Configure Persistent Data   #238
Configure Prompt Template   #226
Configure RAG Account   #227
Configure Region Monitor Script   #185   ⚠ Pro:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Configure Regression Model   #222
Constrain Found Set   #126
Convert File   #139   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Copy   #47   ⚠ WebD:Partial
Copy All Records/Requests   #98   ⚠ WebD:No, DataAPI:No, CWP:No
Copy Record/Request   #101   ⚠ WebD:No, DataAPI:No, CWP:No
Correct Word   #106   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Create Data File   #190   ⚠ WebD:No, DataAPI:No
Create PDF   #243
Cut   #46   ⚠ WebD:Partial
Delete Account   #135
Delete All Records   #10   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Delete File   #197   ⚠ WebD:No, DataAPI:No
Delete Portal Row   #104   ⚠ WebD:Partial, Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Delete Record/Request   #9   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Dial Phone   #65   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Duplicate Record/Request   #8
Edit User Dictionary   #109   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Else   #69
Else If   #125
Enable Account   #137
Enable Touch Keyboard   #174   ⚠ Pro:Partial, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
End If   #70
End Loop   #73
Enter Browse Mode   #55   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Enter Find Mode   #22   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Enter Preview Mode   #41   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Execute FileMaker Data API   #203
Execute SQL   #117   ⚠ Go:No, WebD:Partial, Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Exit Application   #44   ⚠ Go:Partial, WebD:Partial, DataAPI:No, CWP:No
Exit Loop If   #72
Exit Script   #103
Export Field Contents   #132   ⚠ Go:Partial, WebD:Partial, Cloud:No, DataAPI:Partial, CWP:No
Export Records   #36   ⚠ Go:Partial, WebD:Partial, Server:Partial, Cloud:Partial, DataAPI:No, CWP:No
Extend Found Set   #127
Find Matching Records   #155
Fine-Tune Model   #213
Flush Cache to Disk   #102   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Flush Web Viewer Cookies   #237   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Freeze Window   #79   ⚠ Server:No, Cloud:No, DataAPI:No, CWP:No
Generate Response from Model   #220
Get Data File Position   #194   ⚠ WebD:No, DataAPI:No
Get File Exists   #188   ⚠ WebD:No, DataAPI:No
Get File Size   #189   ⚠ WebD:No, DataAPI:No
Get Folder Path   #181   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Go to Field   #17
Go to Layout   #6   ⚠ Pro:Partial, WebD:Partial, Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Go to List of Records   #228   ⚠ Pro:Partial, WebD:Partial, Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Go to Next Field   #4
Go to Object   #145
Go to Portal Row   #99   ⚠ WebD:Partial, Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Go to Previous Field   #5
Go to Record/Request/Page   #16   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Go to Related Record   #74   ⚠ Pro:Partial, WebD:Partial, Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Halt Script   #90
If   #68
Import Records   #35   ⚠ Go:Partial, WebD:Partial, Server:Partial, Cloud:Partial, DataAPI:No, CWP:No
Insert Audio/Video   #159   ⚠ WebD:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Insert Calculated Result   #77
Insert Current Date   #13
Insert Current Time   #14
Insert Current User Name   #60
Insert Embedding   #215
Insert Embedding in Found Set   #216
Insert File   #131   ⚠ Go:Partial, WebD:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Insert from Device   #161   ⚠ Pro:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Insert from Index   #11   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Insert from Last Visited   #12
Insert from URL   #160
Insert Image Caption   #241
Insert Image Captions in Found Set   #240
Insert PDF   #158   ⚠ WebD:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Insert Picture   #56   ⚠ WebD:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Insert Text   #61
Install Menu Set   #142   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Install OnTimer Script   #148   ⚠ Server:No, Cloud:No, DataAPI:No, CWP:No
Install Plug-In File   #157   ⚠ Go:No
Loop   #71
Modify Last Find   #24
Move/Resize Window   #119   ⚠ Go:Partial, WebD:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
New File   #82   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
New Record/Request   #7
New Window   #122   ⚠ Go:Partial, WebD:Partial, CWP:Partial
Omit Multiple Records   #26   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Omit Record   #25
Open Data File   #191   ⚠ WebD:No, DataAPI:No
Open Edit Saved Finds   #149   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Favorites   #183   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open File   #33   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open File Options   #114   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Find/Replace   #129   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Help   #32   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Hosts   #118   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Manage Containers   #156   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Manage Data Sources   #140   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Manage Database   #38   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Manage Layouts   #151   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Manage Themes   #165   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Manage Value Lists   #112   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open PDF   #246   ⚠ WebD:Partial
Open Record/Request   #133
Open Script Workspace   #88   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Settings   #105   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Sharing   #113   ⚠ Go:No, WebD:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Open Transaction   #205
Open Upload To Host   #172   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Open URL   #111   ⚠ WebD:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Paste   #48   ⚠ WebD:Partial
Pause/Resume Script   #62
Perform AppleScript (macOS)   #67   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Perform Find   #28
Perform Find by Natural Language   #221
Perform Find/Replace   #128   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Perform JavaScript in Web Viewer   #175   ⚠ Server:No, Cloud:No, DataAPI:No, CWP:No
Perform Quick Find   #150
Perform RAG Action   #219
Perform Script   #1
Perform Script On Server   #164
Perform Script On Server with Callback   #210   ⚠ Server:No, Cloud:No, DataAPI:No, CWP:No
Perform Semantic Find   #218
Perform SQL Query by Natural Language   #214   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Print   #43   ⚠ Go:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Print PDF   #242   ⚠ Go:Partial, WebD:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Print Setup   #42   ⚠ Go:Partial, WebD:Partial, Server:Partial, Cloud:Partial, DataAPI:No, CWP:No
Re-Login   #138   ⚠ WebD:Partial, Server:Partial, Cloud:No, DataAPI:Partial, CWP:Partial
Read from Data File   #193   ⚠ WebD:No, DataAPI:No
Recover File   #95   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Refresh Object   #167   ⚠ Server:No, Cloud:No, DataAPI:No, CWP:No
Refresh Portal   #180   ⚠ Server:No, Cloud:No, DataAPI:No, CWP:No
Refresh Window   #80
Relookup Field Contents   #40   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Rename File   #199   ⚠ WebD:No, DataAPI:No
Replace Field Contents   #91   ⚠ Go:Partial, WebD:Partial, Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Reset Account Password   #136
Revert Record/Request   #51   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Revert Transaction   #207
Save a Copy as   #37   ⚠ Go:Partial, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Save a Copy as Add-on Package   #96   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Save a Copy as XML   #3   ⚠ Go:No, WebD:No, DataAPI:No, CWP:No
Save Records as Excel   #143   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Save Records as JSONL   #225   ⚠ Go:No, WebD:No
Save Records as PDF   #144   ⚠ Go:Partial, WebD:Partial, Server:Partial, Cloud:Partial, CWP:No
Save Records as Snapshot Link   #152   ⚠ Go:Partial, WebD:Partial, DataAPI:No, CWP:No
Scroll Window   #81   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Select All   #50   ⚠ Go:Partial
Select Dictionaries   #108   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Select Window   #123   ⚠ WebD:Partial
Send DDE Execute (Windows)   #64   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Send Event   #57   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Send Mail   #63   ⚠ Go:Partial, WebD:Partial, Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Set AI Call Logging   #217
Set Data File Position   #195   ⚠ WebD:No, DataAPI:No
Set Dictionary   #209   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Set Error Capture   #86   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Set Error Logging   #200   ⚠ Cloud:No, CWP:No
Set Field   #76
Set Field By Name   #147
Set Layout Object Animation   #168
Set Multi-User   #84   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Set Next Serial Value   #116
Set Revert Transaction on Error   #223
Set Selection   #130   ⚠ Go:Partial, WebD:Partial
Set Session Identifier   #208
Set Use System Formats   #94   ⚠ WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Set Variable   #141
Set Web Viewer   #146   ⚠ WebD:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Set Window Title   #124
Set Zoom Level   #97   ⚠ Go:Partial, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Show All Records   #23
Show Custom Dialog   #87   ⚠ Go:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Show Omitted Only   #27
Show/Hide Menubar   #166   ⚠ Pro:Partial, WebD:Partial, Server:No, Cloud:No, DataAPI:No, CWP:No
Show/Hide Text Ruler   #92   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Show/Hide Toolbars   #29   ⚠ DataAPI:No, CWP:No
Sort Records   #39   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Sort Records by Field   #154
Speak (macOS)   #66   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Spelling Options   #107   ⚠ Go:No, WebD:No, Server:No, Cloud:No, DataAPI:No, CWP:No
Trigger Claris Connect Flow   #211
Truncate Table   #182   ⚠ Server:Partial, Cloud:Partial, DataAPI:Partial, CWP:Partial
Undo/Redo   #45
Unsort Records   #21
View As   #30   ⚠ WebD:Partial
Write to Data File   #192   ⚠ WebD:No, DataAPI:No
```
