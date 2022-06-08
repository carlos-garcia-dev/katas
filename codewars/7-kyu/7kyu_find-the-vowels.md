202205191604
Name: **Find the vowels**
Link: [Codewars](https://www.codewars.com/kata/5680781b6b7c2be860000036)
Level: [[7 kyu]]
Tags: [[Fundamentals]] 

---

# Find the vowels

We want to know the index of the vowels in a given word, for example, there are two vowels in the word super (the second and fourth letters).

So given a string "super", we should return a list of [2, 4].

**Example**:

``` javascript
Some examples:
Mmmm  => []
Super => [2,4]
Apple => [1,5]
YoMama -> [1,2,4,6] javascript
```

Vowels in this context refers to: a e i o u y (including upper case)
This is indexed from `[1..n]` (not zero indexed!)

---

## Solution 1

``` javascript
function vowelIndices(word){
  
  let vowelsList = []
  word
    .toLowerCase()
    .split('')
    .map((e,i,a) => { 
         e === 'a' ? vowelsList.push(i+1) : 
         e === 'e' ? vowelsList.push(i+1) : 
         e === 'i' ? vowelsList.push(i+1) : 
         e === 'o' ? vowelsList.push(i+1) : 
         e === 'u' ? vowelsList.push(i+1) : 
         e === 'y' ? vowelsList.push(i+1) : 
         'a' }) 
  return vowelsList
}
```