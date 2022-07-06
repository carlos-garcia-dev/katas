202207061641
Name: **Summing a number's digits**
Link: [Codewars](https://www.codewars.com/kata/52f3149496de55aded000410/)
Level:  [[Fundamentals]]
Tags: [[7 kyu]]

---

# Summing a number's digits

Write a function named `sumDigits` which takes a number as input and returns the sum of the absolute value of each of the number's decimal digits.

### Examples

``` 
10 --> 1
99 --> 18
-32 --> 5
```

---

## Solution 1

``` javascript
const sumDigits = n => {
  if (n<0) n *= -1
  const numToString = `${n}`.split('')
  return +numToString.reduce((cur,acc)=>+cur + +acc)
}
```

## Solution 2

``` javascript
sumDigits=n=>Math.abs(n).toString().split('').reduce((cur,acc)=>+acc+ +cur, 0)
```