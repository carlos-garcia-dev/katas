202205231901
Name: **Remove First and Last Character**
Link: [Codewars](https://www.codewars.com/kata/56bc28ad5bdaeb48760009b0)
Level:  [[8 kyu]]
Tags: [[Fundamentals]] [[Basic-Language-Features]] [[Strings]]

---

# Remove First and Last Character

It's pretty straightforward. Your goal is to create a function that removes the first and last characters of a string. You're given one parameter, the original string. You don't have to worry with strings with less than two characters.

---

## Solution

``` javascript
removeChar = s => s.slice(1, s.length-1)
```