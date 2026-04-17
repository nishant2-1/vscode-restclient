"Add base64 encoding/decoding system variables"


## Summary
Implements base64 encoding and decoding functionality for REST Client.

## Changes
- Added `$encodeBase64()` system variable
- Added `$decodeBase64()` system variable
- Added regex patterns for proper parsing
- Comprehensive error handling

## Usage
@encoded = {{$encodeBase64(hello world)}} @decoded = {{$decodeBase64(aGVsbG8gd29ybGQ=)}}


Fixes #1431


Summary of All Changes
File	Change
src/common/constants.ts	Add 4 new constants
src/utils/httpVariableProviders/systemVariableProvider.ts	Add 2 regex patterns, 2 methods, 2 constructor calls
Total lines changed: ~15-20 lines

