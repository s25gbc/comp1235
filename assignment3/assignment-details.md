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
Create a JavaScript function that meets the following requirements:
* Authored using arrow expression syntax (constant name calculateSalary)
* Is passed an array of integers, that is ordered from Monday to Sunday
* Every element in the array can be safely assumed to be greater than or equal to 0.
* The function internally must utilize the Array.prototype.reduce() function where the reducer function calculates and returns the calculated total gross weekly salary using the following formula:
  * A worker earns $10 an hour for the first 8 hours
  * For every extra hour worked per day, they earn $15 for each added
  * On weekends, the employer pays double the usual rate, regardless of how many hours worked
    * 10 hours worked on a weekday would pay $80 + $30 = $110
    * 10 hours worked on a weekend would pay $160 + $60 = $220
* The function must pass the following tests at a minimum:

  ```javascript
  calculateSalary([8,8,8,8,8,0,0]) → 400
  calculateSalary([10,10,10,0,8,0,0]) → 410
  calculateSalary([0,0,0,0,0,12,0]) → 280
  ```

---

### Function 3: `indexMultiplier(array)`
Create a JavaScript Arrow function that meets the following requirements:

* Authored using arrow expression syntax (constant name indexMultiplier())
* The function is passed an array of numbers
* The function returns the sum of all items in the array where each item is multiplied by its index
* The function internally must use the Array.prototype.reduce() function to solve this problem.
* The function must pass the following tests at a minimum:

  ```javascript
  indexMultiplier([1, 2, 3, 4, 5]) → 40
  indexMultiplier([-3, 0, 8, -6]) → -2
  indexMultiplier([15, 16, -100, 50]) → -34
  ```

---

### Function 4: `filteredJSON(array)`

Create a JavaScript function that meets the following requirements:
* Authored using arrow expression syntax (constant name filteredJSON())
* Is passed an array of JSON elements
  * The function filters the input array
  * The function returns a new array that contains only those elements in the source whose:
    * id is greater than 10
    * **AND**
    * whose username starts with a character within the range [M-Z] (second half of alphabet)
      * ignore case-sensitivity
* The function internally must utilize the Array.prototype.filter()
* The function must pass the following tests at a minimum:

  ```javascript
  filteredJSON([{id: 1, u: "batman"}]) → []
  filteredJSON([{id: 11, u: "spidey"}]) → [{id: 11, u: "spidey"}]
  filteredJSON([{id: 1, u: "batman"}, {id: 11, u: "spidey"}]) → [{id: 11, u: "spidey"}]
  ```

---

### Function 5: `breakAway(array, n)`

Create a JavaScript function expression that meets the following requirements:
* Authored using **function expression** syntax (with constant name **breakAway**)
* Accepts an array of integers as the first argument, and a single integer as the second argument (n).
* The function divides the array into chunks of size n, where n is the length of each created (divided) array
* It is possible that the last array created is not completely filled (see example 2 below)
* The integers provided in the array argument, and for the value of n, are **always** single-digit integers.
  * validation is **not** required for this single-digit assumption.
* The function returns an array containing the array groupings back to the caller.

  ```javascript
  _breakAway([2,3,4,5], 2) → [ [2,3],[4,5] ]
  _breakAway([2,3,4,5,6], 2) → [ [2,3],[4,5],[6] ]
  _breakAway([2,3,4,5,6,7], 3) → [ [2,3,4],[5,6,7] ]
  _breakAway([2,3,4,5], 1) → [ [2],[3],[4],[5] ]
  _breakAway([2,3,4,5,6,7], 7) → [ [2,3,4,5,6,7] ]
  ```

---
### To Optionally view Test Running on GBLearn:
Optionally upload the following 2 files to GBLearn under the path public_html/comp1235/assignments/assignment3 to see your remote tests running.

1. `solution.js`

   * Contains your 5 function implementations.
2. `index.html`

   * Provided template file.
   * Properly reference your JavaScript file.
   * Uncomment **remote** test script and comment **local** script after local testing.

### How to Submit:

* Please see the link in the GitHub classroom for Submission instructions

### Plagiarism Warning:

* Moss will be used to detect code similarities.
* Zero tolerance policy.

---


**GOOD LUCK!**
