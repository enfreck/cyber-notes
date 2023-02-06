Another reverse engineering tool - good for dynamic analysis

## ida \<file.exe\>

### Display Values in registers during execution
1. Set a breakpoint in the blocks
2. Run
3. Press `g` and type in a register name 
4. Press `a` for ascii

### Enable Tracing
1. Set breakpoint
2. Edit breakpoint
3. Enable Tracing
4. Play
5. Instructions executed are highlighted in yellow

### Force Execution Down a Path
1. Set breakpoint
2. Edit breakpoint
3. Set condition (ex. ZF=0)
4. Uncheck Break (so execution doesn't halt at that breakpoint)
OR
1. Right click on an instruction and Set IP --> The program will start executing from there

### Patch Binary
1. BACK UP BINARY (cp binary.exe copy.exe)
2. 
