202204250743
Name: Beginner Series #3 Sum of Numbers
Link: [Codewars](https://www.codewars.com/kata/55f2b110f61eb01779000053)
Level: [[7 kyu]]
Tags: [[Fundamentals]] [[Algorithms]]

---

# Beginner Series #3 Sum of Numbers

Given two integers `a` and `b`, which can be positive or negative, find the sum of all the integers between and including them and return it. If the two numbers are equal return `a` or `b`.

**Note:** `a` and `b` are not ordered!

**Examples:**

```
(1, 0) --> 1 (1 + 0 = 1)
(1, 2) --> 3 (1 + 2 = 3)
(0, 1) --> 1 (0 + 1 = 1)
(1, 1) --> 1 (1 since both are same)
(-1, 0) --> -1 (-1 + 0 = -1)
(-1, 2) --> 2 (-1 + 0 + 1 + 2 = 2)
```

---

## Solution

``` javascript
// Solution 1
function getSum(n1,n2) {
  if(n1===n2) return n1
  const group = [n1,n2].sort((a,b)=>a-b)
  let result = []
  for(let i=group[0]; i<= group[1]; i++){ result.push(i)}  
  return result.reduce((acc,cur)=>acc+cur)
}

// Solution 2
getSum=(a,b)=>(Math.abs(a-b)+1)*(a+b)/2
```