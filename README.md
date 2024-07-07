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
|9101|is it equal the number|
|9102|is it lessthan the number|
|9103|logical not the number|
|9201|read memory's value|
|9202|write value in memory|
|9203|swap top 2 value on stack|
|9204|pop stack's top value|
|9301|set value of program counter|
|9302|jump if condtion is true|
|9303|Non processing|
|9401|shutdown computer|
|9402|output as UTF-8 characher |

## Example
This program to addition 5987 and 8762 write result in memory. 
```
9 9201 10 9201 9001 11 9203 9202 9401 5987 8762 0
```
This program to counting up until number become 5. 
```
15 9201 1 9001 15 9203 9202 15 9201 5 9101 9103 0 9302 9401 0
```
