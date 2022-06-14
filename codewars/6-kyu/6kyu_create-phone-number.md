202206141635
Name: **Create Phone Number**
Link: [Codewars](https://www.codewars.com/kata/525f50e3b73515a6db000b83)
Level:  [[6 kyu]]
Tags: [[Arrays]] [[Strings]] [[Formatting]] [[Regular Expressions]] [[Algorithms]]

---

# Phone Number

Write a function that accepts an array of 10 integers (between 0 and 9), that returns a string of those numbers in the form of a phone number.

**Example**:

``` javascript
createPhoneNumber([1, 2, 3, 4, 5, 6, 7, 8, 9, 0]) // => returns "(123) 456-7890"
```

The returned format must be correct in order to complete this challenge.  
Don't forget the space after the closing parentheses!

---

## Solution

``` javascript
createPhoneNumber=arr=>arr.join('').replace(/(\d{3})(\d{3})(\d{4})/,'($1) $2-$3')
```