202206091617
Name: **Count characters in your string**
Link: [Codewars]()
Level:  [[6 kyu]]
Tags: [[Strings]] [[Fundamentals]]

---

# Count characters in your string

The main idea is to count all the occurring characters in a string. If you have a string like aba, then the result should be {'a': 2, 'b': 1}.

What if the string is empty? Then the result should be empty object literal, {}.


---

## Solution

``` javascript
const count = s => {  
  let object = {}s.split('').map(e=>object[e]=object[e]+1||1)
  return object
}
```
