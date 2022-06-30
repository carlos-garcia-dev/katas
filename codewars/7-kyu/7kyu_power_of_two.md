202206301756
Name: **Power of two**
Link: [Codewars](https://www.codewars.com/kata/534d0a229345375d520006a0)
Level:  [[7 kyu]]
Tags: [[Mathematics]] [[Algorithms]] [[Fundamentals]]

---

# Power of two

Complete the function power_of_two/powerOfTwo (or equivalent, depending on your language) that determines if a given non-negative integer is a power of two. From the corresponding Wikipedia entry:

a power of two is a number of the form 2n where n is an integer, i.e. the result of exponentiation with number two as the base and integer n as the exponent.

You may assume the input is always valid.

## Examples

``` javascript
isPowerOfTwo(1024) // -> true
isPowerOfTwo(4096) // -> true
isPowerOfTwo(333)  // -> false
```

---

## Solution

``` javascript
isPowerOfTwo = n => Number.isInteger(Math.log2(n))
```