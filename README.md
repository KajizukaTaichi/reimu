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
|9101|compare is it equal the number|
|9102|compare is it lessthan the number|
|9103|logical not the number|
|9201|read memory's value|
|9202|write value in memory|
|9203|swap top 2 value on the stack|
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
0 1 9001 0 9203 9202 0 9201 5 9101 9103 0 9302 9401
```
This program to output "Hello, world!" message.
```
72 9402 101 9402 108 9402 108 9402 111 9402 44 9402 32 9402 119 9402 111 9402 114 9402 108 9402 100 9402 33 9402 9401
```