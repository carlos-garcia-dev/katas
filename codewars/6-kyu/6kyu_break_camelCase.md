202206301715
Name: **Break camelCase**
Link: [Codewars](https://www.codewars.com/kata/5208f99aee097e6552000148)
Level:  [[6 kyu]]
Tags: [[Strings]] [[Formatting]] [[Fundamentals]]

---

# Break camelCase

Complete the solution so that the function will break up camel casing, using a space between words.

## Example

```
"camelCasing"  =>  "camel Casing"
"identifier"   =>  "identifier"
""             =>  ""
```

---

## Solution

``` javascript
solution=s=>s.replace(/([A-Z])/g, ' $1')
```