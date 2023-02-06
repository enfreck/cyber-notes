Compiles C programs
Addiitonal Resources: http://gcc.gnu.org/onlinedocs/

## gcc \<file.c\>
Basic compilation.  Output is listed as `a.out`.  Execute program by `a.out <parameters>`

## gcc -o \<executable_name\> \<file.c\>
`-o`  allows you to specify the name you want to be given to the executable

## gcc -o <executable_name> -Wall <file.c>
`-Wall` displays all warnings when compiling
`-Wformat`  displays warnings regarding mistmatches between format specifiers and arguments
`-Wunused`  displays warnings regarding unused variables
`-Wimplicit`  displays warnings regarding functions that are called withoout being declared
`-Wconversion`  displays warnings regarding implicit conversions that could result in errirs
`-Wshadow`  displays warnings regarding name hiding
`-W`  a variety of additional warnings not included in `-Wall`

## gcc -o <executable_name> -Wall -std=c11 <file.c>
`-std=c11` directs gcc to require code to comply with C11 language standard


