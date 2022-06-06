202206061427
Name: **Find the missing letter**
Link: [Codewars]()
Level:  [[6 kyu]]
Tags: [[Mathematics]] [[Algorithms]]

---

# Find the missing letter

Write a method that takes an array of consecutive (increasing) letters as input and that returns the missing letter in the array.

You will always get an valid array. And it will be always exactly one letter be missing. The length of the array will always be at least 2.  
The array will always contain letters in only one case.

**Example**:

```javascript
["a","b","c","d","f"] -> "e"
["O","Q","R","S"] -> "P"
```


---

## Solution

``` javascript
const findMissingLetter = arr => String.fromCharCode(
    arr
      .find((c, i) => arr[i + 1].charCodeAt() - c.charCodeAt() !== 1)
      .charCodeAt() + 1
  )
```