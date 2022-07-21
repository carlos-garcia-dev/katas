202207081753
Name: **Fix string case**
Link: [Codewars](https://www.codewars.com/kata/5b180e9fedaa564a7000009a)
Level:  [[7 kyu]]
Tags: [[Fundamentals]]

---

# Fix string case

In this Kata, you will be given a string that may have mixed uppercase and lowercase letters and your task is to convert that string to either lowercase only or uppercase only based on:

-   make as few changes as possible.
-   if the string contains equal number of uppercase and lowercase letters, convert the string to lowercase.

### Example:

```
solve("coDe") = "code". Lowercase characters > uppercase. Change only the "D" to lowercase.
solve("CODe") = "CODE". Uppercase characters > lowecase. Change only the "e" to uppercase.
solve("coDE") = "code". Upper == lowercase. Change all to lowercase.
```

---

## Solution

``` javascript
const solve = s => {
  const upperCase = s.split('').filter(e=>e.match(/[A-Z]/)).length
  const lowerCase = s.split('').filter(e=>e.match(/[a-z]/)).length
  return lowerCase >= upperCase ? s.toLowerCase() : s.toUpperCase()
}
```