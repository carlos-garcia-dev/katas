202206091616
Name: **Count the divisors of a number**
Link: [Codewars](https://www.codewars.com/kata/542c0f198e077084c0000c2e)
Level:  [[7kyu]]
Tags:  [[Strings]] [[Fundamentals]]

---

# Anagram Detection

An **anagram** is the result of rearranging the letters of a word to produce a new word (see [wikipedia](https://en.wikipedia.org/wiki/Anagram)).

**Note:** anagrams are case insensitive

Complete the function to return `true` if the two arguments given are anagrams of each other; return `false` otherwise.

**Examples**:

"foefet" is an anagram of "toffee"

"Buckethead" is an anagram of
"DeathCubeK"

---

## Solution 1

``` javascript
const isAnagram = (s1,s2) => {
  const original = s1.toLowerCase().split('').sort().join('')
  const result = s2.toLowerCase().split('').sort().join('')
  return original === result
}
```

## Solution 2

``` javascript
const sortWord=w=>w.toLowerCase().split('').sort().join('')
const isAnagram=(s1,s2)=>sortWord(s1)===sortWord(s2)
```
