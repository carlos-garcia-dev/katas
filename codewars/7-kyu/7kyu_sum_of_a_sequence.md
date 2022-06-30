202206301748
Name: **Sum of a sequence**
Link: [Codewars](https://www.codewars.com/kata/586f6741c66d18c22800010a)
Level:  [[7 kyu]]
Tags: [[Fundamentals]] [[Recursion]]

---

# Sum of a sequence

Your task is to make function, which returns the sum of a sequence of integers.

The sequence is defined by 3 non-negative values: **begin**, **end**, **step (inclusive)**.

If **begin** value is greater than the **end**, function should returns **0**

## Examples

``` javascript
2,2,2 --> 2
2,6,2 --> 12 (2 + 4 + 6)
1,5,1 --> 15 (1 + 2 + 3 + 4 + 5)
1,5,3  --> 5 (1 + 4)
```

---

## Solution

``` javascript
const sequenceSum = (b,e,s) => {
  if (b > e) return 0
  let array = []
  for (let i=b; i <= e; i +=s) {
    array.push(i)
  }
  return array.reduce((cur,acc)=>cur+acc, 0)
}
```