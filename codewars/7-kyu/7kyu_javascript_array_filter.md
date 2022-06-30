202206301739
Name: **JavaScript Array Filter**
Link: [Codewars](https://www.codewars.com/kata/514a6336889283a3d2000001)
Level:  [[7 kyu]]
Tags: [[Arrays]] [[Fundamentals]]

---

# JavaScript Array Filter

JavaScript Arrays support a filter function (starting in JavaScript 1.6). Use the filter functionality to complete the function given.

## Example

``` javascript
getEvenNumbers([2,4,5,6]) // should == [2,4,6]
```

---

## Solution 1

``` javascript
 getEvenNumbers=arr=>arr.filter(n=>!(n%2))
```

## Solution 2

``` javascript
getEvenNumbers = arr => arr.filter( n => n % 2 === 0 )
```