# Reimu
Simple and efficientive stack model virtual machine.
Built on Stack technology.

## Command set 
9000 series value is use as program

|command|behave|
|-|-|
|9001|addition the number|
|9002|subtraction the number|
|9003|multiprication the number|
|9004|division the number|
|9005|modulo the number|
|9006|power the number|
|9011|read memory's value|
|9012|write value in memory|
|9013|swap top 2 value on stack|
|9014|pop stack's top value|
|9015|set value of program counter|
|9091|shutdown computer|

## Example
This program to addition 5987 and 8762 write result in memory. 
```
9 9011 10 9011 9001 11 9013 9012 9091 5987 8762 0
```
This program to counting up forever. 
```
0 1 9001 1 9015
```
