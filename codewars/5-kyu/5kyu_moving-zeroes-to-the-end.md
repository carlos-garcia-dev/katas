202204171516
Name: **Moving Zeros To The End**
Link: [Codewars](https://www.codewars.com/kata/52597aa56021e91c93000cb0)
Level:  [[5 kyu]]
Tags: [[Algorithms]] [[Interviews]] [[Arrays]] [[Sorting]]

---

# Moving Zeros To The End

Write an algorithm that takes an array and moves all of the zeros to the end, preserving the order of the other elements.

```javascript
moveZeros([false,1,0,1,2,0,1,3,"a"]) // returns[false,1,1,2,1,3,"a",0,0]
```

---

## Solution

``` javascript
 moveZeros=arr=>{
    const zeroes  = arr.filter(n=>n===0),
    ordered = arr.filter(n=>n!==0)
    return ordered.concat(zeroes)
 }
```