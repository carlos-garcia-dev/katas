202206141638
Name: **Highest Scoring Word**
Link: [Codewars](https://www.codewars.com/kata/57eb8fcdf670e99d9b000272)
Level:  [[6 kyu]]
Tags: [[Fundamentals]] [[Strings]] [[Arrays]]

---

# Highest Scoring Word

Given a string of words, you need to find the highest scoring word.

Each letter of a word scores points according to its position in the alphabet: `a = 1, b = 2, c = 3` etc.

You need to return the highest scoring word as a string.

If two words score the same, return the word that appears earliest in the original string.

All letters will be lowercase and all inputs will be valid.

---

## Solution

``` javascript
high=s=>{
  let as = s
    .split(" ")
    .map(w => [...w].reduce((a,b)=>a+b.charCodeAt(0)-96, 0))
  return s.split(" ")[as.indexOf(Math.max(...as))];
}
```