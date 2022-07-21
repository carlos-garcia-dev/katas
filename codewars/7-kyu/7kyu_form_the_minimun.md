202207081757
Name: **Form The Minimum**
Link: [Codewars]()
Level:  [[7 kyu]]
Tags: [[Fundamentals]]

---

# Form The Minimum

**_Given_** a **_list of digits_**, _return the **_smallest number_** that could be formed from these digits, using the digits only once (ignore duplicates).

Only **_positive integers_** _will be passed to the function (> 0 ), no negatives or zeros.

### Example

```
minValue ({1, 3, 1})  ==> return (13)
```

---

## Solution

``` javascript
minValue=arr=>+Array.from(new Set(arr)).sort((a,b)=>a-b).join('')
```