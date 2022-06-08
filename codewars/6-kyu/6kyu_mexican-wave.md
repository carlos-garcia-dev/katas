202206081810
Name: **Mexican Wave**
Link: [Codewars](https://www.codewars.com/kata/58f5c63f1e26ecda7e000029/)
Level:  [[6 kyu]]
Tags: [[Fundamentals]] [[Algorithms]] [[Arrays]]

---

# Mexican Wave

In this simple Kata your task is to create a function that turns a string into a Mexican Wave. You will be passed a string and you must return that string in an array where an uppercase letter is a person standing up.

**Example**:

``` javascript
wave("hello") => ["Hello", "hEllo", "heLlo", "helLo", "hellO"]
```

---

## Solution

``` javascript
const wave = str => {
  let result = []
  
  for(let i=0; i < str.length ; i++){
    let letters = str.split('')
    if(letters[i] !== ' ') {
      letters[i] = letters[i].toUpperCase()
      result.push(letters.join(''))  
    }
  }
  return result
}
```