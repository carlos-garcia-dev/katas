202206301743
Name: **Two Oldest Ages**
Link: [Codewars](https://www.codewars.com/kata/511f11d355fe575d2c000001)
Level:  [[7 kyu]]
Tags: [[Arrays]] [[Algorithms]]

---

# Two Oldest Ages

The order of the numbers passed in could be any order. The array will always include at least 2 items. If there are two or more oldest age, then return both of them in array format.

## Example

``` javascript
[1, 2, 10, 8] --> [8, 10]
[1, 5, 87, 45, 8, 8] --> [45, 87]
[1, 3, 10, 0]) --> [3, 10]
```

---

## Solution

``` javascript
const twoOldestAges=arr=> arr.sort((a,b)=>b-a).slice(0,2).sort((a,b)=>a-b)
```