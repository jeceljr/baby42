# baby42

This simple RISC processor is meant to have educational value rather than be practical. Its name is based on the fact that it deals with 4 byte wide data (32 bits) and has 2 byte wide instructions (16 bits).

A key design goal was that it should be nice to program in assembly language and even the hexadecimal version of its machine language should be easy to learn. If programs are going to be developed in C or Python then the details for the processor don't matter and there is no point in having something other than an AVR8, x86, ARM or RISC-V.

Being typical has some educational value, and this processor is a typical load/store architecture with 16 registers. It doesn't have a status register, but that is also the case for some other RISCs.

Being non typical also has educational value since students can see that there are different ways of doing things. The exclusive use of skips for conditional execution and the use of "cascades" to combine pairs of operations is unusual. The algebra-style syntax for the assembly is pretty different.

The same design allows slight variations like baby22 (16 bit data, 16 bit instructions) and baby042 (24 bit data and 12 bit instructions).

Currently there are no implementation files, only [slides for a quick presentation](doc/baby42_slides.pdf) in the doc subdirectory. The slides include some assembly language examples near the end.
