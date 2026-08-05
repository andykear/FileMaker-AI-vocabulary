```text
# FileMaker Pro function reference, compressed. Target: FileMaker 26. Every function below is valid at this version.
# This is the authoritative function list. Rules:
# - Only use functions that appear below. Never invent a function.
# - Parameter order is authoritative. Optional parameters are shown in { }.
# - If a required function is not listed here, state that no such FileMaker function exists rather than guessing.
# - Aggregate functions (Sum, Count, Average, Max, Min, StDev, StDevP, Variance, VarianceP) take '{; field...}' as shown,
#   but each field slot also accepts: a repeating field; a related field (table::field); a comma-free list of several fields
#   (field1;field2;...); matching-record lists including across tables (table1::a;table2::b). The signature shows the canonical form.

Abs ( number ) → number, time
Acos ( number ) → number
AddEmbeddings ( v1 ; v2 ) → text, container
Asin ( number ) → number
Atan ( number ) → number
Average ( field {; field...} ) → number
Base64Decode ( text {; fileNameWithExtension } ) → text, container
Base64Encode ( data ) → text
Base64EncodeRFC ( RFCNumber ; data ) → text
BaseTableComment ( fileName ; baseTableName ) → text
BaseTableIDs ( fileName ) → text
BaseTableNames ( fileName ) → text
Case ( test1 ; result1 {; test2 ; result2 ; ... ; defaultResult } ) → text, number, date, time, timestamp, container
Ceiling ( number ) → number
Char ( number ) → text
Choose ( test ; result0 {; result1 ; result2...} ) → text, number, date, time, timestamp, container
Code ( text ) → number
Combination ( setSize ; numberOfChoices ) → number
ComputeModel ( modelName ; parameterName1 ; value1 {; parameterName2 ; value2 ...} ) → text
ComputeModel ( modelName ; "image" ; value1 ; "confidenceLowerLimit" ; returnAtLeastOne ) → text
ConvertFromFileMakerPath ( filemakerPath ; format ) → text
ConvertToFileMakerPath ( standardPath ; format ) → text
Cos ( angleInRadians ) → number
CosineSimilarity ( v1 ; v2 ) → number
Count ( field {; field...} ) → number
CryptAuthCode ( data ; algorithm ; key ) → container
CryptDecrypt ( container ; key ) → text, container
CryptDecryptBase64 ( text ; key ) → text, container
CryptDigest ( data ; algorithm ) → container
CryptEncrypt ( data ; key ) → container
CryptEncryptBase64 ( data ; key ) → text
CryptGenerateSignature ( data ; algorithm ; privateRSAKey ; keyPassword ) → container
CryptVerifySignature ( data ; algorithm ; publicRSAKey ; signature ) → number
DatabaseNames → text
Date ( month ; day ; year ) → date
Day ( date ) → number
DayName ( date ) → text
DayNameJ ( date ) → text
DayOfWeek ( date ) → number
DayOfYear ( date ) → number
Degrees ( angleInRadians ) → number
Div ( number ; divisor ) → number
Evaluate ( expression {; [field1 ; field2 ;...]} ) → text, number, date, time, timestamp, container
EvaluationError ( expression ) → number
Exact ( originalText ; comparisonText ) → number
ExecuteSQL ( sqlQuery ; fieldSeparator ; rowSeparator { ; arguments... } ) → text
ExecuteSQLe ( sqlQuery ; fieldSeparator ; rowSeparator { ; arguments... } ) → text
Exp ( number ) → number
Extend ( non-repeatingField ) → text, number, date, time, timestamp, container
Factorial ( number {; numberOfFactors } ) → number
FieldAnnotation ( fileName ; fieldName ) → text
FieldBounds ( fileName ; layoutName ; fieldName ) → text
FieldComment ( fileName ; fieldName ) → text
FieldDisplayNames ( fileName ; fieldName ) → text
FieldIDs ( fileName ; layoutName ) → text
FieldNames ( fileName ; layoutName ) → text
FieldRepetitions ( fileName ; layoutName ; fieldName ) → text
FieldStyle ( fileName ; layoutName ; fieldName ) → text
FieldType ( fileName ; fieldName ) → text
Filter ( textToFilter ; filterText ) → text
FilterValues ( textToFilter ; filterValues ) → text
Floor ( number ) → number
Furigana ( text {; option } ) → text
FV ( payment ; interestRate ; periods ) → number
Get ( AccountExtendedPrivileges ) → text
Get ( AccountGroupName ) → text
Get ( AccountName ) → text
Get ( AccountPasswordDaysRemaining ) → number
Get ( AccountPrivilegeSetName ) → text
Get ( AccountType ) → text
Get ( ActiveFieldContents ) → text, number, date, time, timestamp, container
Get ( ActiveFieldName ) → text
Get ( ActiveFieldTableName ) → text
Get ( ActiveLayoutObjectName ) → text
Get ( ActiveModifierKeys ) → number
Get ( ActivePortalRowNumber ) → number
Get ( ActiveRecordNumber ) → number
Get ( ActiveRepetitionNumber ) → number
Get ( ActiveSelectionSize ) → number
Get ( ActiveSelectionStart ) → number
Get ( AllowAbortState ) → number
Get ( AllowFormattingBarState ) → number
Get ( ApplicationArchitecture ) → Text
Get ( ApplicationLanguage ) → text
Get ( ApplicationVersion ) → text
Get ( CacheFileName ) → text
Get ( CacheFilePath ) → text
Get ( CalculationRepetitionNumber ) → number
Get ( ConnectionAttributes ) → text
Get ( ConnectionState ) → number
Get ( CurrentDate ) → date
Get ( CurrentExtendedPrivileges ) → text
Get ( CurrentHostTimestamp ) → timestamp
Get ( CurrentPrivilegeSetName ) → text
Get ( CurrentTime ) → time
Get ( CurrentTimestamp ) → timestamp
Get ( CurrentTimeUTCMicroseconds ) → number, time
Get ( CurrentTimeUTCMilliseconds ) → number, time
Get ( CustomMenuSetName ) → text
Get ( DesktopPath ) → text
Get ( Device ) → number
Get ( DocumentsPath ) → text
Get ( DocumentsPathListing ) → text
Get ( EncryptionState ) → text
Get ( ErrorCaptureState ) → number
Get ( FileLocaleElements ) → text
Get ( FileMakerPath ) → text
Get ( FileName ) → text
Get ( FilePath ) → text
Get ( FileSize ) → number
Get ( FoundCount ) → number
Get ( GuidedAccessState ) → number
Get ( HighContrastState ) → number
Get ( HostApplicationVersion ) → text
Get ( HostIPAddress ) → text
Get ( HostName ) → text
Get ( InstalledFMPlugins ) → text
Get ( InstalledFMPluginsAsJSON ) → text
Get ( LastError ) → number
Get ( LastErrorDetail ) → text
Get ( LastErrorLocation ) → text
Get ( LastMessageChoice ) → number
Get ( LastStepTokensUsed ) → text
Get ( LayoutAccess ) → number
Get ( LayoutCount ) → number
Get ( LayoutName ) → text
Get ( LayoutNumber ) → number
Get ( LayoutTableName ) → text
Get ( LayoutViewState ) → number
Get ( MenubarState ) → number
Get ( ModifiedFields ) → text
Get ( MultiUserState ) → number
Get ( NetworkProtocol ) → text
Get ( NetworkType ) → number
Get ( OpenDataFileInfo ) → text
Get ( PageCount ) → number
Get ( PageNumber ) → number
Get ( PersistentID ) → text
Get ( PreferencesPath ) → text
Get ( PrinterName ) → text
Get ( QuickFindText ) → text
Get ( RecordAccess ) → number
Get ( RecordID ) → number
Get ( RecordModificationCount ) → number
Get ( RecordNumber ) → number
Get ( RecordOpenCount ) → number
Get ( RecordOpenState ) → number
Get ( RegionMonitorEvents ) → text
Get ( RequestCount ) → number
Get ( RequestOmitState ) → number
Get ( RevertTransactionOnErrorState ) → number
Get ( ScreenDepth ) → number
Get ( ScreenHeight ) → number
Get ( ScreenScaleFactor ) → number
Get ( ScreenWidth ) → number
Get ( ScriptAnimationState ) → number
Get ( ScriptName ) → text
Get ( ScriptParameter ) → text, number, date, time, timestamp, container
Get ( ScriptResult ) → text, number, date, time, timestamp, container
Get ( SessionIdentifier ) → text
Get ( SortState ) → number
Get ( StatusAreaState ) → number
Get ( SystemAppearance ) → text
Get ( SystemDrive ) → text
Get ( SystemIPAddress ) → text
Get ( SystemLanguage ) → text
Get ( SystemLocaleElements ) → text
Get ( SystemNICAddress ) → text
Get ( SystemPlatform ) → number
Get ( SystemStorageAvailable ) → number
Get ( SystemVersion ) → text
Get ( TemporaryPath ) → text
Get ( TextRulerVisible ) → number
Get ( TotalRecordCount ) → number
Get ( TouchKeyboardState ) → number
Get ( TransactionOpenState ) → number
Get ( TriggerCurrentPanel ) → text
Get ( TriggerExternalEvent ) → number
Get ( TriggerGestureInfo ) → text
Get ( TriggerKeystroke ) → text
Get ( TriggerModifierKeys ) → number
Get ( TriggerTargetPanel ) → text
Get ( UserCount ) → number
Get ( UserName ) → text
Get ( UseSystemFormatsState ) → number
Get ( UUID ) → text
Get ( UUIDNumber ) → number
Get ( WindowContentHeight ) → number
Get ( WindowContentWidth ) → number
Get ( WindowDesktopHeight ) → number
Get ( WindowDesktopWidth ) → number
Get ( WindowHeight ) → number
Get ( WindowLeft ) → number
Get ( WindowMode ) → number
Get ( WindowName ) → text
Get ( WindowOrientation ) → number
Get ( WindowStyle ) → number
Get ( WindowTop ) → number
Get ( WindowUUID ) → text
Get ( WindowVisible ) → number
Get ( WindowWidth ) → number
Get ( WindowZoomLevel ) → text
GetAddonInfo ( addonID ) → text
GetAsBoolean ( data ) → number
GetAsCSS ( text ) → text
GetAsDate ( text ) → date
GetAsNumber ( text ) → number
GetAsSVG ( text ) → text
GetAsText ( data ) → text
GetAsTime ( text ) → time
GetAsTimestamp ( text ) → timestamp
GetAsURLEncoded ( text ) → text
GetAVPlayerAttribute ( attributeName ) → text, number
GetBaseTableName ( field ) → text
GetContainerAttribute ( field ; attributeName ) → text, number, date, time, timestamp, container
GetEmbedding ( account ; model ; input ) → container
GetEmbeddingAsFile ( text {; fileNameWithExtension } ) → container
GetEmbeddingAsText ( data ) → text
GetField ( fieldName ) → text, number, date, time, timestamp, container
GetFieldName ( field ) → text
GetFieldsOnLayout ( layoutName ) → text
GetHeight ( field ) → number
GetLayoutObjectAttribute ( objectName ; attributeName {; repetitionNumber ; portalRowNumber } ) → text
GetLayoutObjectOwnerInfo ( objectID ) → text
GetLiveText ( container ; language ) → text
GetLiveTextAsJSON ( container ; language ) → text
GetModelAttributes ( modelName ) → text
GetNextSerialValue ( fileName ; fieldName ) → text
GetNthRecord ( field ; recordNumber ) → text, number, date, time, timestamp, container
GetPersistentData ( name ; instanceID ) → text, number, date, time, timestamp, container
GetRAGSpaceInfo ( ragAccountName {; spaceID } ) → text
GetRecordIDsFromFoundSet ( type { ; tableOccurrenceOrPortal } ) → text
GetRepetition ( repeatingField ; number ) → text, number, date, time, timestamp, container
GetSensor ( sensorName {; option1 ; option2 } ) → text, number
GetSummary ( summaryField ; breakField ) → number, date, time, timestamp
GetTableDDL ( tableOccurrenceNames ; ignoreError ) → text
GetTextFromPDF ( container ) → text
GetThumbnail ( field ; width ; height ) → container
GetTokenCount ( text ) → number
GetValue ( listOfValues ; valueNumber ) → text
GetWidth ( field ) → number
HexDecode ( data {; fileNameWithExtension } ) → text, container
HexEncode ( data ) → text
Hiragana ( text ) → text
Hour ( time ) → number
If ( test ; result1 {; result2 } ) → text, number, date, time, timestamp, container
Int ( number ) → number
IsEmpty ( field ) → number
IsValid ( field ) → number
IsValidExpression ( expression ) → number
JSONDeleteElement ( json ; keyOrIndexOrPath ) → text
JSONFormatElements ( json ) → text
JSONGetElement ( json ; keyOrIndexOrPath ) → text, number
JSONGetElementType ( json ; keyOrIndexOrPath ) → text, number
JSONListKeys ( json ; keyOrIndexOrPath ) → text
JSONListValues ( json ; keyOrIndexOrPath ) → text
JSONMakeArray ( listOfValues ; separator ; type ) → text
JSONParse ( json ) → text
JSONParsedState ( json ) → number
JSONSetElement ( json ; keyOrIndexOrPath ; value ; type ) → text
JSONSetElement ( json ; [key1 ; value1 ; type1] {; [key2 ; value2 ; type2] ; ... [keyN ; valueN ; typeN]} ) → text
KanaHankaku ( text ) → text
KanaZenkaku ( text ) → text
KanjiNumeral ( text ) → text
Katakana ( text ) → text
Last ( repeatingField ) → text, number, date, time, timestamp, container
LayoutIDs ( fileName ) → text
LayoutNames ( fileName ) → text
LayoutObjectNames ( fileName ; layoutName ) → text
LayoutObjectUUID → text
Left ( text ; numberOfCharacters ) → text
LeftValues ( text ; numberOfValues ) → text
LeftWords ( text ; numberOfWords ) → text
Length ( text ) → number
Let ( {[} var1 = expression1 {; var2 = expression2...]} ; calculation ) → text, number, date, time, timestamp, container
Lg ( number ) → number
List ( field {; field...} ) → text
ListPersistentDataIDs ( name ) → text
Ln ( number ) → number
Location ( accuracy {; timeout } ) → Text
LocationValues ( accuracy {; timeout } ) → Text
Log ( number ) → number
Lookup ( sourceField {; failExpression } ) → text, number, date, time, timestamp, container
LookupNext ( sourceField ; lower/higherFlag ) → text, number, date, time, timestamp, container
Lower ( text ) → text
Max ( field {; field...} ) → text, number, date, time, timestamp
Middle ( text ; start ; numberOfCharacters ) → text
MiddleValues ( text ; startingValue ; numberOfValues ) → text
MiddleWords ( text ; startingWord ; numberOfWords ) → text
Min ( field {; field...} ) → text, number, date, time, timestamp
Minute ( time ) → number
Mod ( number ; divisor ) → number
Month ( date ) → number
MonthName ( date ) → text
MonthNameJ ( date ) → text
NormalizeEmbedding ( data { ; dimension } ) → text, container
NPV ( payment ; interestRate ) → number
NumToJText ( number ; separator ; characterType ) → text
PatternCount ( text ; searchString ) → number
Pi → number
PMT ( principal ; interestRate ; term ) → number
Position ( text ; searchString ; start ; occurrence ) → number
PredictFromModel ( modelName ; v1 ) → number
Proper ( text ) → text
PV ( payment ; interestRate ; periods ) → number
Quote ( text ) → text
Radians ( angleInDegrees ) → number
Random → number
RangeBeacons ( UUID {; timeout ; major ; minor } ) → Text
ReadQRCode ( container ) → text
RelationInfo ( fileName ; tableName ) → text
Replace ( text ; start ; numberOfCharacters ; replacementText ) → text
RGB ( red ; green ; blue ) → number
Right ( text ; numberOfCharacters ) → text
RightValues ( text ; numberOfValues ) → text
RightWords ( text ; numberOfWords ) → text
RomanHankaku ( text ) → text
RomanZenkaku ( text ) → text
Round ( number ; precision ) → number
ScriptIDs ( fileName ) → text
ScriptNames ( fileName ) → text
Seconds ( time ) → number
Self → text, number, date, time, timestamp
SerialIncrement ( text ; incrementBy ) → text
SetPrecision ( expression ; precision ) → number
SetRecursion ( expression ; maxIterations ) → text, number, date, time, timestamp, container
Sign ( number ) → number
Sin ( angleInRadians ) → number
SortValues ( values {; datatype ; locale } ) → text
Sqrt ( number ) → number
StDev ( field {; field...} ) → number
StDevP ( field {; field...} ) → number
Substitute ( text ; searchString ; replaceString ) → text
Substitute ( text ; [search1 ; replace1] {; [search2 ; replace2] ; ... [searchN ; replaceN]} ) → text
SubtractEmbeddings ( v1 ; v2 ) → text, container
Sum ( field {; field...} ) → number
TableIDs ( fileName ) → text
TableNames ( fileName ) → text
Tan ( angleInRadians ) → number
TextColor ( text ; RGB ( red ; green ; blue ) ) → text
TextColorRemove ( text {; RGB ( red ; green ; blue )} ) → text
TextDecode ( container ; encoding ) → text
TextEncode ( text ; encoding ; lineEndings ) → container
TextFont ( text ; fontName ) → text
TextFontRemove ( text {; fontToRemove } ) → text
TextFormatRemove ( text ) → text
TextSize ( text ; fontSize ) → text, number
TextSizeRemove ( text {; sizeToRemove } ) → text
TextStyleAdd ( text ; styles ) → text
TextStyleRemove ( text ; styles ) → text
Time ( hours ; minutes ; seconds ) → time
Timestamp ( date ; time ) → timestamp
Trim ( text ) → text
TrimAll ( text ; trimSpaces ; trimType ) → text
Truncate ( number ; precision ) → number
UniqueValues ( values {; datatype ; locale } ) → text
Upper ( text ) → text
ValueCount ( text ) → number
ValueListIDs ( fileName ) → text
ValueListItems ( fileName ; valueList ) → text
ValueListNames ( fileName ) → text
Variance ( field {; field...} ) → number
VarianceP ( field {; field...} ) → number
VerifyContainer ( field ) → text
WeekOfYear ( date ) → number
WeekOfYearFiscal ( date ; startingDay ) → number
While ( [ initialVariable ] ; condition ; [ logic ] ; result ) → text, number, date, time, timestamp, container
WindowNames {( fileName )} → text
WordCount ( text ) → number
Year ( date ) → number
YearName ( date ; format ) → text
```
