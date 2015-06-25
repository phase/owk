# owk
Owk is a compiled, esoteric, golfing, register-based, programming language that runs on the FVM. It is compiled into FVM bytecode, which can be put through the FVM for results.

Owk is parsed line by line. You can make a "fake" line by putting a `;`. Comments are parked by `#` and are only at the start of a line, and whitespace is ignored.

```python
a=7
6=84
#The same as
a = 7; 6 = 84
```

There are 16 registers in total, each marked by their [hexadecimal counterpart](https://en.m.wikipedia.org/wiki/Hexadecimal#Using_0.E2.80.939_and_A.E2.80.93F). To load a number to these registers, we use `=`. (It basically overwrites whatever was in the register before.)

```python
#Loads 8 to register f
f=8
#You can also use capitals
F=8
```

You can also do your normal math operations in Owk using the registers.

```python
#Adds the values of registers a & f and stores it in register e
a+f>e
#Multiplies 2 & d and stores it in f
2*d>f
```
