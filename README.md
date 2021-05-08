MONEY
=====

By Rhea Myers.

A simple BBC BASIC program to output a very short series of statements of
different relationships to money (money.bbc), and an even shorter version
in a more modern dialect of BBC BASIC (modern-money.bbc).

Run in a BBC Micro emulator or a BBC BASIC interpreter.

e.g.:
```
$ bbcbasic
BBC BASIC for Linux Console v0.32
(C) Copyright R. T. Russell, 2021
>LOAD "money.bbc"
>LIST
   10 DIM word$(3)
   20 word$(1)="FUCK"
   30 word$(2)="YOU"
   40 word$(3)="MONEY"
   50 FOR i=1 TO 3
   60   FOR j=1 TO 3
   70     PRINT word$(j);
   80     IF j=i THEN PRINT ", "; ELSE PRINT " ";
   90   NEXT j
  100   PRINT
  110 NEXT i
>RUN
FUCK, YOU MONEY 
FUCK YOU, MONEY 
FUCK YOU MONEY, 
>
```
