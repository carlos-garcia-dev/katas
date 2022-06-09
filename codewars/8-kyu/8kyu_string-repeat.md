202205231902
Name: **String repeat**
Link: [Codewars](https://www.codewars.com/kata/57a0e5c372292dd76d000d7e)
Level: [[8 kyu]]
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