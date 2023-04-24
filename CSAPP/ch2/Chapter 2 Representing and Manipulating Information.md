# Chapter 2 Representing and Manipulating Information

Modern computers store and process information represented as two-valued signals. 

We consider the three most important representations of numbers. 

-   *Unsigned encodings* are based on traditional binary notation, representing numbers greater than of equal to 0. 
-   *Two’s-complement* encodings are the most common way to represent *signed* integers, that is, numbers that may be either positive or negative.
-   *Floating-point* encodings are a base-2 version of scientific notation for representing real numbers.

Computer representations use a limited number of bits to encode a number, and hence some operations can *overflow* when the results are too large to be represented.

Integer representations can encode a comparatively small range of values, but do so precisely, while floating-point representations can encode a wide range of values, but only approximately.

## 2.1 Information Storage

Rather than accessing individual bits in memory, most computers use blocks of 8 bits, or *bytes*, as the smallest addressable unit of memory. 

A machine-level program views memory  as a very large array of bytes, referred to as *virtual memory*. 

Every byte of memory is identified by a unique number, known as its *address*, and the set of all possible address is known as the *virtual address space*. 

### 2.1.1 Hexadecimal Notation

