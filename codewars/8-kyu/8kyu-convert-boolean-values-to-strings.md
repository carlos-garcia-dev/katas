202205241014
Name:  **Convert boolean values to strings 'Yes' or 'No'**
Link: [Codewars](https://www.codewars.com/kata/53369039d7ab3ac506000467)
Level:  [[8 kyu]]
Tags: [[Fundamentals]] [[Booleans]] [[Best-Practices]]

---

# Convert boolean values to strings 'Yes' or 'No'.

Complete the method that takes a boolean value and return a `"Yes"` string for `true`, or a `"No"` string for `false`.

---

## Solution

``` javascript
boolToWord=b=>b?'Yes':'No'
```

## Solution 2

``` javascript
boolToWord=b=>b===true?'Yes':'No'
```