202204250736
Name: Is this a triangle?
Link: [Codewars](https://www.codewars.com/kata/56606694ec01347ce800001b)
Level: [[7 kyu]]  
Tags: [[Fundamentals]] [[Mathematics]] [[Algorithms]] [[Numbers]] [[Utilities]]

---

# Is this a triangle?

Implement a function that accepts 3 integer values a, b, c. The function should return true if a triangle can be built with the sides of given length and false in any other case.

(*In this case, all triangles must have surface greater than 0 to be accepted*).

---

## Solution

``` javascript
isTriangle=(a,b,c)=>a-b<c && b-c<a && c-a<b
```
