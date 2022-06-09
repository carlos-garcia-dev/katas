202205232155
Name: **Square(n) Sum**
Link: [Codewars](https://www.codewars.com/kata/515e271a311df0350d00000f)
Level: [[8 kyu]]
Tags: [[Fundamentals]] [[Arithmetic]] [[Mathematics]] [[Algorithms]] [[Numbers]] [[Arrays]] [[Lists]] [[Data-Structures]]

---

# Square(n) Sum

Complete the square sum function so that it squares each number passed into it and then sums the results together.

For example, for `[1, 2, 2]` it should return `9` because `1^2 + 2^2 + 2^2 = 9`.

---

## Solution

``` javascript
squareSum=n=>n.map(e=>e**2).reduce((acc,cur)=>acc+cur, 0)
```
