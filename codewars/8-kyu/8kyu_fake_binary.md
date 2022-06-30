202206301719
Name: **Fake Binary**
Link: [Codewars]()
Level:  [[8 kyu]]
Tags: [[Fundamentals]] [[Strings]] [[Arrays]]

---

# Fake Binary

Given a string of digits, you should replace any digit below 5 with '0' and any digit 5 and above with '1'. Return the resulting string.

**Note: input will never be an empty string**

---

## Solution

``` javascript
fakeBin=x=>x.split('').map(n=>n>=5?1:0).join('')
```