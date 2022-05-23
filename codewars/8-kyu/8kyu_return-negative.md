202205232031
Name:  **Return Negative**
Link: [Codewars](https://www.codewars.com/kata/55685cd7ad70877c23000102)
Level:  [[8 kyu]]
Tags: [[Fundamentals]] [[Numbers]]

---

#   Return Negative

In this simple assignment you are given a number and have to make it negative. But maybe the number is already negative?

``` javascript
makeNegative(1);    // return -1
makeNegative(-5);   // return -5
makeNegative(0);    // return 0
makeNegative(0.12); // return -0.12
```

**Notes**:

-   The number can be negative already, in which case no change is required.
-   Zero (0) is not checked for any specific sign. Negative zeros make no mathematical sense.

---

## Solution

``` javascript
makeNegative=n=>n!==0?-Math.abs(n):n
```
