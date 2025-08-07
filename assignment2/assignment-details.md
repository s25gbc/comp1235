# COMP1235 Assignment 2
## Introduction to Full Stack Development

---

## Assignment Details

**Assignment Type:** Individual Assignment

### Description
In this assignment, you are to develop a JavaScript file (`solution.js`) that contains the implementation of 5 functions. Each function is represented as one step, and marks will be awarded on the completion of each step (each function).

Each function is independent and solves a unique problem, as such, treat and implement each function in isolation of the others, that is, you should only focus on one problem at a time.

**PLEASE NOTE:** Unless indicated within the question(s), input validation is NOT required for a functions input parameters – You may assume that all input parameters provided to your functions, are valid.

### Objective
- Write decision-making statements and control structures to solve problems
- Apply programming logic to solve basic to intermediate problems
- Testing and debugging

### Learning Outcomes
After conducting this assignment students will/will be able to:
1. Acquainted with implementing JavaScript functions
2. Follow instructions, and to implement various requirements
3. Acquainted with authoring JavaScript unit tests to validate their functions

**You are NOT permitted to use any external files or libraries. Using any external libraries will result in a final grade of ZERO for your assignment submission.**

3. Your JavaScript functions file must be configured for strict mode (`"use strict"`)

---

## Function 1: Find the Number of Digits in an Argument
### `_findNumOfDigits(arg)`

Create a JavaScript function that meets the following requirements:

- Is passed an argument (arg)
- The function determines the number of digits in the argument
  - The length of the argument (number of characters) varies
- The function returns the count of the number of digits back to the caller.

**Expected Output:**
```javascript
_findNumOfDigits(1000)      → 4
_findNumOfDigits("abcd")    → 0
_findNumOfDigits(12)        → 2
_findNumOfDigits("COMP1235") → 4
_findNumOfDigits(0)         → 1
_findNumOfDigits("C1O2M3P5") → 4
```

---

## Function 2: Surplus Function
### `_surplus(str)`

Create a JavaScript function that meets the following requirements:

- The function takes a string argument (str).
- The function returns a function, that returns the original str argument

**This means that you can save that function into a variable and then return that variable**

**Expected Output:**
```javascript
_surplus("orange") → inner() → orange
_surplus("pear")   → inner() → pear
_surplus("")       → inner() → ""
```

---

## Function 3: Strings with Numbers
### `_strNumbers(array)`

Create a JavaScript function that meets the following requirements:

- Receives an array of strings (source array)
  - Some of the strings in the source array have numbers, some do not
  - The strings in the array vary in length
- Returns a new array that contains the strings, from the source array, that contained numbers in them.
- If there are no strings in the source array, then the function returns and empty array
- If there are strings in the source array, but none of them contain numbers, then the function returns an empty array to the caller.

**Expected Output:**
```javascript
numInStr(["1a", "a", "2b", "b"])                      → ["1a", "2b"]
numInStr(["abc", "abc10"])                             → ["abc10"]
numInStr(["abc", "ab10c", "a10bc", "bcd"])             → ["ab10c", "a10bc"]
numInStr(["this is a test", "test1"])                  → ["test1"]
```

---

## Function 4: Class Grading
### `_determineClassGrading(array)`

Create a JavaScript function that meets the following requirements:

- Receives a variable length array of numbers, representing student grades in a course
- The function traverses the array to determine the number of passing and failing grades.
  - A passing grade, is grade greater than or equal to 50
- The function displays the count (console log) for the number passing grades, failing grades and overall class average as illustrated below
- Average class grade is rounded to 1 decimal point
- The function returns the array containing the number of passing grades, the number of failing grades, and the overall averages of the grades, respectively, back to the caller

**Expected Output:**
```javascript
_determineClassGrading([50,51,80,45])    → [3,1,56.5]
_determineClassGrading([35,45,25,10,6,33]) → [0,6,25.7]
_determineClassGrading([80,90])          → [2,0,85.0]
```

---

## Function 5: Move Capital Letters
### `_moveCapitalLetters`

Create a JavaScript Arrow function that meets the following requirements:

- Authored using arrow expression syntax (constant name `_moveCapitalLetters`)
- That takes in a string parameter, of mixed casing (mix of upper and lowercase letters)
- The function moves all capital letters to the front of a word.
- The uppercase letters moved to the front, maintain their original relative order
- The lowercase letters moved to the back front, maintain their original relative order
- Console log output is NOT permitted.
- The function should pass each of the illustrated examples below at a minimum.

**Expected Output:**
```javascript
_moveCapitalLetters("hApPy")     → "APhpy"
_moveCapitalLetters("moveMENT")  → "MENTmove"
_moveCapitalLetters("shOrtCAKE") → "OCAKEshrt"
```

---

## Submission Procedure and Rules

Please ensure to remove all instances of the following from your final submission solution:
- any commented code
- Do not over use the console log, spamming the console log unnecessarily, say for example with debug related output may cost you marks.

### Submission Procedure

Please refer to [Development and Submissions Instructions](https://github.com/s25gbc/comp1235/blob/main/assignment2/development-and-submissions-instructions.md) for further instructions.

### Additional Submission Requirements

Late submissions are graded at a penalty per day (five day maximum) **-20%**

We are going to use Moss (https://theory.stanford.edu/~aiken/moss/) to detect similarities in code among all students. There will be zero tolerance for plagiarism. Please be aware.

---

**GOOD LUCK!**
