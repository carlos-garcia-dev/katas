202206091637
Name: **Weird String Case**
Link: [Codewars](https://www.codewars.com/kata/52b757663a95b11b3d00062d)
Level:  [[6 kyu]]
Tags: [[Strings]] [[Algorithms]]

---

# Weird String Case

Write a function toWeirdCase (weirdcase in Ruby) that accepts a string, and returns the same string with all even indexed characters in each word upper cased, and all odd indexed characters in each word lower cased. The indexing just explained is zero based, so the zero-ith index is even, therefore that character should be upper cased and you need to start over for each word.

The passed in string will only consist of alphabetical characters and spaces(' '). Spaces will only be present if there are multiple words. Words will be separated by a single space(' ').

**Examples**:

``` javascript
toWeirdCase( "String" );//=> returns "StRiNg"
toWeirdCase( "Weird string case" );//=> returns "WeIrD StRiNg CaSe"
```

---

## Solution

``` javascript
toWeirdCase=s=>s.split(' ').map((e,i)=>e.split('').map((e,i)=>i%2===0?e.toUpperCase():e.toLowerCase()).join('')).join(' ')
```