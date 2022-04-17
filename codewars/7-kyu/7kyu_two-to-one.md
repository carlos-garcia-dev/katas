202204171040
Name: Two to One
Link: [Codewars](https://www.codewars.com/kata/5656b6906de340bd1b0000ac)
Level:  [[7 kyu]]
Tags: [[Fundamentals]]

---

# Two to One

Take 2 strings `s1` and `s2` including only letters from `a`to `z`. Return a new **sorted** string, the longest possible, containing distinct letters - each taken only once - coming from s1 or s2.

**Examples:**

```js
 a = "xyaabbbccccdefww"
 b = "xxxxyyyyabklmopq"
 longest(a, b) -> "abcdefklmopqwxy"

 a = "abcdefghijklmnopqrstuvwxyz"
 longest(a, a) -> "abcdefghijklmnopqrstuvwxyz"
```

---

## Solution

**Solution 1**

``` javascript
longest=(s1,s2)=>s1.concat(s2).split('').filter((elm,idx,arr)=>arr.indexOf(elm)===idx).sort().join('')
```

**Solution 2**

```js
longest=(s1,s2)=>[...new Set(s2+s1)].sort().join('')
```

### Resources