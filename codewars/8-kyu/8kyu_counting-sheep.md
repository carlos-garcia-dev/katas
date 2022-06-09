202205232158
Name: **Counting sheep...**
Link: [Codewars](https://www.codewars.com/kata/54edbc7200b811e956000556)
Level: [[8 kyu]]
Tags: [[Fundamentals]] [[Arrays]]

---

# Counting sheep...

Consider an array/list of sheep where some sheep may be missing from their place. We need a function that counts the number of sheep present in the array (true means present).

Example:

```javascript
[true,  true,  true,  false,
  true,  true,  true,  true ,
  true,  false, true,  false,
  true,  false, false, true ,
  true,  true,  true,  true ,
  false, false, true,  true]
```

The correct answer would be `17`.

Hint: Don't forget to check for bad values like `null`/`undefined`

---

## Solution

``` javascript
function countSheeps(arr) {
  let sheeps = []
  arr.map(e=>e===true?sheeps.push(e):sheeps)
  return sheeps.length
}
```


## Solution 2

``` javascript
countSheeps=arr=>arr.filter(Boolean).length
```