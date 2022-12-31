# SB-fantasy-cpu-emulator
A GitHub repository for my Small Basic CPU emulator code and other things.
________________________________
This CPU emulator does not emulate any excisting CPUs.
It currently has the following instructions:

NOP - no operation

ITM - immediate to memory

PUSH M - push value at memory[address] to stack

PUSH I push immediate to stack

POP - pop value at stack[stackpointer] to memory[address]

DLY I - delay with immediate

DLY M - delay with value at memory[address]

DLY S - delay with value at stack[stackpointer]

JMP I - jump to address immediate

JMP M - jump to address memory[address]

JMP S - jump to address stack[stackpointer]

COMP M M - compare value at memory[a1] with memory[a2], store the results at memory[a3]

COMP I I - compare immediate value1 with compare immediate value2, store the results at memory[a1]

COMP M I - compare immediate value with value at memory[a1], store the results at memory[a1]

COMP I M - compare value at memory[a1] with immediate value, store the results at memory[a1]

            //the results:
            
            0 if value1 is smaller than value2
            
            1 if value1 is equal to value2
            
            2 if value1 is bigger than value2
            
            
JS - jump to a2 if memory[a1] is 0

JE - jump to a2 if memory[a1] is 1

JB - jump to a2 if memory[a1] is 2

JNS - jump to a2 if memory[a1] is not 0

JNE - jump to a2 if memory[a1] is not 1

JNB - jump to a2 if memory[a1] is not 2

INC - increment value at memory[address] by 1

DEC - decrement value at memory[address] by 1

PRNT I - print immediate value without new line

PRNTL I - print immediate value with new line

PRNT M - print value at memory[address] without new line

PRNTL M - print value at memory[address] with new line

PRNT S - print value at stack[stackpointer] without new line

PRNTL S - print value at stack[stackpointer] with new line

RNG - generate random number(integer) with a maximum value of a1, store at memory[a1]

HALT - halts the program
_________________________
The user update(v0.5): new instructions:
__________________________

EXE I - opens a new program, ram and stack file where the program rom's name is immidiate value 1, the ram's is IV2, the stack's is IV3

EXE M - opens a new program, ram and stack file, where the program rom's name is at memory[a1], the ram's at memory[a2], the stack's at memory[a3]

CLR D - clears console

INP S - gets a srting input from user, saves the input at stack[stackpointer]

NINP S - gets a number input from user, saves the input at stack[stackpointer]

INP M - gets a srting input from user, saves the input at memory[address]

NINP M - gets a number input from user, saves the input at memory[address]
________________________
Inportant notes:

I do not even know if this is an emulator or a compiler or somthing else. At the time of making this repository, I'm only 14 years old, that's why this is written in Small Basic, which is not even recognised by GitHub as a programming languauge.

The  expension.txt file contains debug code. For usage, it needs to be put in the main while loop, after the "oper" variable decleration.
