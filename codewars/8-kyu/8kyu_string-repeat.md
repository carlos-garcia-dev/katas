202205231902
Name: **String repeat**
Link: [Codewars]()
Level:  [[8 kyu]]
Tags: [[Fundamentals]]

---

# String repeat

Write a function called `repeatStr` which repeats the given string `string` exactly `n` times.

``` javascript
repeatStr(6, "I") // "IIIIII"
repeatStr(5, "Hello") // "HelloHelloHelloHelloHello"
```

---

## Solution

``` javascript
repeatStr=(n,s)=>s.repeat(n)
```