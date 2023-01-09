Allows a user to step through the execution of a program

## Compiling Program
In order to use gdb's features, generally you want to 
- disable optimization by using `-O0`
- enable the generation of extra debugging information by using `-g` or `-ggdb3`

Ex. `gcc -o matloff -std=c11 -O0 -Wall -W -ggdb3 matloff.c`   ([gcc](../gcc.md))

## Run gdb
`gdb <executable>` 

## Commands
`run`  Run program
`backtrace`  Information on how you arrived at an error
`list`  Display source code
`kill`  Stop running process
`print <var>`  Print value of a variable
`p <var>`  Print value of a variable
`p/x <var>`  Print value of variable as hex
`p (char) <var>`  Print variable as a char
`break <function name>`  Set a breakpoint at the beginning of a function
`break <filename.c:<linenumber>`  Set a breakpoint at a certain line
`break <filename.c>:<linenumber> if <condition>`  Set a breakpoint at a certain line when the line is reached and the condition is true
`next`  Step through program one line at a time
`n`  Step through program one line at a time
`step`  Into a function call
`disassem`  Assembly code of a function
`ni`  Step through assembly instruction code



