202204211348
Name: Reverse words
Link: [Codewars](https://www.codewars.com/kata/5259b20d6021e9e14c0010d4)
Level:  [[7 kyu]]
Tags: [[Fundamentals]] [[Strings]]

---

# Reverse words

Complete the function that accepts a string parameter, and reverses each word in the string. **All** spaces in the string should be retained.

## Examples

```
"This is an example!" ==> "sihT si na !elpmaxe"
"double  spaces"      ==> "elbuod  secaps"
``````

---

## Solution

``` javascript
reverseWords=s=>s.split(" ").map(e=>e.split("").reverse().join("")).join(" ")
```