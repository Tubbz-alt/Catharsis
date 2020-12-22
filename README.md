 Catharsis

 A parasitic meltdown worm
 Coded by 'HaZel' Timo Sarkar
 Mostly compiled by gcc with C as host language

 General sheet of characteristics:
    Name of the virus.............: Catharsis
    Author........................: Timo 'HaZeL' Sarkar / December 2020
    Size..........................: On 1st generation: aprox. 16800 bytes
    Targets.......................: Linux only... sorry for that
    Encrypted.....................: No
    Polymorphic...................: Yes
    Metamorphic...................: Yes
    Payloads......................: Yes: Stdout

 To do in next versions: Find bugs and add more comments / work on KASLR

 To build locally:
    $ nasm -fwin32 catharsis.asm
    $ gcc catharsis.obj -o catharsis.out
    $ chmod a+x catharsis.out
    $ ./catharsis.out

 Quick reference (keyword search):
    Variable declaration........................: $define && equ
    Beginning of virus..........................: .main:
    Meltdown....................................: .dbload:
    Cache-resulation............................: .resolution

(c) Timo Sarkar HaZeL, somewhere on December 2020                         

 DISCLAIMER

 This code is only for research and educational purposes only. The assembling
 of this file will produce a fully functional virus, so you have been warned.
 If this kind of material is illegal in your country or state, you should
 remove it from your computer. The author of this virus declines any illegal
 activity performed by the possesor of the assembled form of this source code
 including possesion and/or spreading of the virus generated from this source
 code.

This source code is provided "as is". The deliberated modification of this
source code will derive in a new virus that must not be considered the virus
sourced here. The author of the original source code will not be considered
the author of the new modified or derivated virus.

