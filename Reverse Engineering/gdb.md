Allows a user to step through the execution of a program

## Compiling Program
In order to use gdb's features, generally you want to 
- disable optimization by using `-O0`
- enable the generation of extra debugging information by using `-g` or `-ggdb3`

Ex. `gcc -o matloff -std=c11 -O0 -Wall -W -ggdb3 matloff.c`   ([gcc](Terminal%20Commands/gcc.md))

**Make sure you have executable permissions before you run gdb** ([chmod](Terminal%20Commands/chmod.md))

## Run gdb x86-64
`gdb <executable>` 
`gdb -q <executable>`  Gets rid of the annoying beginning gdb stuff

## Run arm
*Note: Must split terminal*
`qemu-arm -g 12345 <file.exe>`   
`gdb-multiarch <file.exe>` 
	`gdb> target remote localhost:12345`
	`gdb> disassemble main`
	`gdb> break *main`
	`gdb> continue`

## Commands
`run`  Run program
`backtrace`  Information on how you arrived at an error
`list`  Display source code
`kill`  Stop running process
`print <var>`  Print value of a variable
`p <var>`  Print value of a variable
`p/x <var>`  Print value of variable as hex
`p (char) <var>`  Print variable as a char
`break <function name> (b)`  Set a breakpoint at the beginning of a function
`break <filename.c:<linenumber>`  Set a breakpoint at a certain line
`break <filename.c>:<linenumber> if <condition>`  Set a breakpoint at a certain line when the line is reached and the condition is true
`next (n)`  Step through program one line at a time, going OVER functions
`step (s)`  Step through program one line at a time, going INTO functions
`nexti (ni)`  Step through assembly one instruction at a time, going OVER functions
`stepi (si)`  Step through program one instruction at a time, going INTO functions
`disassemble <function> (disas)`  Assembly code of a function
`x/<format> *<address>` Examines memory at address 
	`x/x *0x401000`  Examines memory at address 0x401000 as a hexadecmal integer
	`x/s $r0`  Examines memory pointed to by the register r0 as a string
	`x/4x $r0`  Examines 4 bytes of memory pointed to by the register r0 as a hexadecimal integer 
`quit`  Exit gdb
`-ex "gcore <file>"` Dump process memory to file  (Ex: -ex "gcore 7-process.core" = Dump process memory to file: 7-process.core)
`-ex starti <.exe>`  Load process 



