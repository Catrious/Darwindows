# DarWindows
A translation layer for Windows to run Darwin binaries. <br>
Darwindows is similar to Darling, although it runs natively on Windows. <br>
WARNING: Darwindows is in alpha stages and supports only some Darwin apps. <br>
NOTE: To use GUI on DarWindows, you need to call 0x2000999 for message box or 0x2000999A for text box. <br>
## Usage
Regular: `darwindows <file>` <br>
Debug: `darwindows --debug <file>` <br>
## Compile from source
### Compile DarWindows
1. Install Go if you don't have it
2. Download the source of DarWindows
3. Run `go build .` in a terminal
### Compile samples
1. Install Zig/Clang if you don't have it
2. Download the code of the sample
3. Run this in your terminal depending on what you have <br>
   Zig: `zig cc <file> -o <output> -target x86_64-macos -nostdlib -ffreestanding` <br>
   Clang: `clang <file> -o <output> -target x86_64-apple-darwin -nostdlib -ffreestanding`
