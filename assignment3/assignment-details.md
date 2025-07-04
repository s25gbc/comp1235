# Assignment 3 - Details

**Assignment Type**: Individual Assignment

---

## 1. Description

You are to develop a JavaScript file (`solution.js`) that implements **5 independent functions**. Each function solves a distinct problem. Input validation is **not required** unless explicitly stated.

---

## 2. Objectives

* Write decision-making statements and control structures.
* Apply programming logic to solve problems.
* Test and debug JavaScript code.

---

## 3. Learning Outcomes

* Implement JavaScript functions.
* Follow technical instructions and requirements.
* Write unit tests to validate function outputs.

---

## 4. Instructions

1. Update the solutions file: `solutions.js`
2. Implement all 5 functions inside this file.
3. Use **strict mode**: `"use strict"`.
5. **No external libraries** are allowed. Using them will result in a grade of zero.

---

## 5. Functions to Implement

### Function 1: `Circle(radius)`
Create a JavaScript function that meets the following requirements:

* The function is function constructor for circle objects (creates and returns circles)
* The Circle constructor accepts a radius (r) as an argument
* Circle has two methods:

  * `area()` – calculates the area (use `Math.PI`, rounded to 2 decimals)
  * `perimeter()` – returns the circumference (rounded to 2 decimals)

* The function must pass the following tests at a minimum:

  ```javascript
  new Circle(3) → c.area()→ 28.27
                → c.perimeter() → 18.85
  new Circle(7) → c.area()→ 153.94
                → c.perimeter()→ 43.98
  new Circle(9) → c.area()→ 254.47
                → c.perimeter()→ 56.55
  ```

---

### Function 2: `calculateSalary(array)`

* Arrow function.
* Takes an array of 7 integers (Mon-Sun hours).
* Uses `Array.prototype.reduce()`.
* Rules:

  * Weekdays: \$10/hour for first 8 hours, \$15/hour after.
  * Weekends: double rate on all hours.

**Example Outputs:**

```javascript
calculateSalary([8,8,8,8,8,0,0]) → 400
calculateSalary([10,10,10,0,8,0,0]) → 410
calculateSalary([0,0,0,0,0,12,0]) → 280
```

---

### Function 3: `indexMultiplier(array)`

* Arrow function.
* Uses `Array.prototype.reduce()`.
* Returns sum of each element multiplied by its index.

**Example Outputs:**

```javascript
indexMultiplier([1, 2, 3, 4, 5]) → 40
indexMultiplier([-3, 0, 8, -6]) → -2
indexMultiplier([15, 16, -100, 50]) → -34
```

---

### Function 4: `filteredJSON(array)`

* Arrow function.
* Filters and returns a new array based on these rules:

  * `id` > 10
  * `username` starts with \[M-Z] (case-insensitive)
* Uses `Array.prototype.filter()`

**Example Outputs:**

```javascript
filteredJSON([{id: 1, u: "batman"}]) → []
filteredJSON([{id: 11, u: "spidey"}]) → [{id: 11, u: "spidey"}]
```

---

### Function 5: `breakAway(array, n)`

* Function expression.
* Accepts array of integers and chunk size `n`.
* Splits the array into subarrays of length `n`.
* Last subarray may be shorter.

**Example Outputs:**

```javascript
breakAway([2,3,4,5], 2) → [[2,3],[4,5]]
breakAway([2,3,4,5,6], 2) → [[2,3],[4,5],[6]]
breakAway([2,3,4,5], 1) → [[2],[3],[4],[5]]
```

---

## 6. Submission Procedure and Rules

### Do Not Include:

* `document.write()`
* `innerHTML()`
* `alert()`
* Excessive `console.log()`

### Files to Submit:

1. `<STUDENT_ID>-problems.js`

   * Contains your 5 function implementations.
2. `index.html`

   * Provided template file.
   * Properly reference your JavaScript file.
   * Uncomment **remote** test script and comment **local** script after local testing.
3. `tests.js`

   * Used to create your own unit tests.

### Upload to:

* `my.gblearn.com → comp1235/assignment 3`
* `public_html/comp1235/assignments/assignment3/`

### Plagiarism Warning:

* Moss will be used to detect code similarities.
* Zero tolerance policy.

---

## 7. Marking Rubric

* **40%** Code and Functionality
* **40%** Logic
* **20%** Best Practices
  * Descriptive variable/function names using camelCase
  * Use `let`/`const` instead of `var`
  * Avoid global variables
  * Consistent and clean coding style

---

**GOOD LUCK!**
