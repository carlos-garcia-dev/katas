202207061635
Name: **Remove anchor from URL**
Link: [Codewars](https://www.codewars.com/kata/51f2b4448cadf20ed0000386/)
Level:  [[7 kyu]]
Tags: [[Regular Expressions]] [[Strings]] [[Fundamentals]]

---

# Remove anchor from URL

Complete the function/method so that it returns the URL with anything after the anchor (`#`) removed.

###  Examples:

```
"www.codewars.com#about" --> "www.codewars.com"
"www.codewars.com?page=1" -->"www.codewars.com?page=1"
```

---

## Solution 1

``` javascript
removeUrlAnchor=s=>s.split('#').slice(0,1).join('')
```

## Solution 2

``` javascript
removeUrlAnchor=s=>s.split('#')[0]
```