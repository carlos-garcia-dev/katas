202206301758
Name: **Greet Me**
Link: [Codewars](https://www.codewars.com/kata/535474308bb336c9980006f2)
Level:  [[7 kyu]]
Tags: [[Strings]] [[Fundamentals]]

---

# Greet Me

Write a method that takes one argument as name and then greets that name, capitalized and ends with an exclamation point.

``` javascript
"riley" --> "Hello Riley!"
"JACK"  --> "Hello Jack!"
```

---

## Solution

``` javascript
greet=n=>`Hello ${n.slice(0,1).toUpperCase()+n.slice(1,n.length).toLowerCase()}!`
```