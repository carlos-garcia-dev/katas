202206091609
Name: **Count the divisors of a number**
Link: [Codewars](https://www.codewars.com/kata/542c0f198e077084c0000c2e)
Level:  [[7kyu]]
Tags: [[Number-theory]] [[Mathematics]] [[Fundamentals]]

---

# Count the divisors of a number

Count the number of divisors of a positive integer `n`.

Random tests go up to `n = 500000`.
**Examples**:

``` javascript
4 --> 3 (1, 2, 4)
5 --> 2 (1, 5)
12 --> 6 (1, 2, 3, 4, 6, 12)
30 --> 8 (1, 2, 3, 5, 6, 10, 15, 30)
```

---

## Solution

``` javascript
const getDivisorsCnt=n=>{
  let divisors = []
  for(let i=1; i <= n; i++){
    if(n%i===0||n===i){
      divisors.push(i) 
    }
  }
  return divisors.length
}
```