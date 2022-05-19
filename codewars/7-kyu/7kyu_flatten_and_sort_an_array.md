202205191604
Name: Flatten and sort an array
Link: [Codewars]()
Level: [[7 kyu]]
Tags: [[Fundamentals]] [[Arrays]] [[Sorting]] [[Algorithms]] [[Lambdas]] [[Funtional-prgramming]] [[Functions]] [[Declarative-Programming]] [[Control-Flow]] [[Basic-Language-Features]]

---

# Flatten and sort an array

Given a two-dimensional array of integers, return the flattened version of the array with all the integers in the sorted (ascending) order.

**Example**:

Given `[[3, 2, 1], [4, 6, 5], [], [9, 7, 8]]`, your function should return `[1, 2, 3, 4, 5, 6, 7, 8, 9]`.

**Addendum**:

Please, keep in mind, that JavaScript is by default sorting objects alphabetically. For more information, please consult:

[StackOverflow - Docs](http://stackoverflow.com/questions/6093874/why-doesnt-the-sort-function-of-javascript-work-well)

---

## Solution 1

``` javascript
const flattenAndSort = arr => {
  const parsed = arr.reduce((acc, num)=>acc.concat(num), [])
  return parsed.sort((a,b)=>a-b)
}
```


## Solution 2 (E2019)

``` javascript
const flattenAndSort = arr => {
  const parsed = arr.flat()
  return parsed.sort((a,b)=>a-b)
}
```