202206301752
Name: **Check the exam**
Link: [Codewars](https://www.codewars.com/kata/5a3dd29055519e23ec000074)
Level:  [[7 kyu]]
Tags: [[Fundamentals]] [[Arrays]] [[Basic-Language-Features]] [[Language-Features]]

---

# Check the exam

The first input array is the key to the correct answers to an exam, like ["a", "a", "b", "d"]. The second one contains a student's submitted answers.

The two arrays are not empty and are the same length. Return the score for this array of answers, giving +4 for each correct answer, -1 for each incorrect answer, and +0 for each blank answer, represented as an empty string (in C the space character is used).

If the score < 0, return 0.

## Example

``` javascript
checkExam(["a", "a", "b", "b"], ["a", "c", "b", "d"]) → 6
checkExam(["a", "a", "c", "b"], ["a", "a", "b",  ""]) → 7
checkExam(["a", "a", "b", "c"], ["a", "a", "b", "c"]) → 16
checkExam(["b", "c", "b", "a"], ["",  "a", "a", "c"]) → 0
```

---

## Solution

``` javascript
const checkExam=(sol,ans)=>{
  let results = []
  ans.map((e,i)=>{
    if(e!==sol[i] && e!== '') results.push(-1)
    if(e===sol[i]) results.push(4)
  })
  results = results.reduce((acc,cur)=>acc+cur,0)
  return results <= 0 ? 0 : results 
}
```