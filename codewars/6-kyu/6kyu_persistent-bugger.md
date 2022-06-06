202206061402
Name: **Persistent Bugger**
Link: [Codewars]()
Level:  [[6 kyu]]
Tags: [[Fundamentals]]

---

# Persistent Bugger

Write a function, `persistence`, that takes in a positive parameter `num` and returns its multiplicative persistence, which is the number of times you must multiply the digits in `num` until you reach a single digit.

**Example**:

``` javascript

39 --> 3 (because 3*9 = 27, 2*7 = 14, 1*4 = 4 and 4 has only one digit)
999 --> 4 (because 9*9*9 = 729, 7*2*9 = 126, 1*2*6 = 12, and finally 1*2 = 2)
4 --> 0 (because 4 is already a one-digit number)
```

---

## Solution

``` javascript
// Soution 1
const persistence = n => {
  return `${n}`.length > 1 
    ? 1 + persistence(`${n}`.split('').reduce((cur,acc) => +cur * +acc))
  	: 0
}
```

``` javascript
// Solution 2
const persistence=n=>`${n}`.length > 1?1+persistence(`${n}`.split('').reduce((cur,acc)=>+cur*+acc):0
```