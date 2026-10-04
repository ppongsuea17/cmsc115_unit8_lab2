# Reflection – AI Number Program Lab

##  Student Name:
Photsavat Pongsuea

##  GitHub Repository Link:
(Insert your repository URL here)

## Iteration 1

What the AI code does:
- The AI-generated code loops through the integer array, adds all of the values together, and returns the sum.

Tests passed/failed:
- testEmptyArray passed. testBasicArray, testNegativeNumbers, and testSingleValue failed.

What surprised you:
- I was surprised that the AI-generated code looked correct at first, but three of the four JUnit tests failed. The tests showed that findResult was not supposed to return the sum of the array.

Commit message:
- Iteration 1: AI-generated implementation

---

## Iteration 2

What changed:
- I changed findResult so it returns the largest integer in the array instead of adding all the values together.

What improved:
- Three of the four JUnit tests passed. The method now correctly handles a normal array, negative numbers, and a single-value array.

What still failed and why:
- The empty array test still failed with an ArrayIndexOutOfBoundsException because the method tries to access values[0] when the array is empty.

Commit message:
- Iteration 2: largest value implementation

---

## Iteration 3

Final behavior of the program:
- The program returns the largest integer in the array. If the array is empty, it returns Integer.MIN_VALUE.

What was fixed:
- I added a check for an empty array before accessing values[0]. This prevents the ArrayIndexOutOfBoundsException that occurred during Iteration 2.

What you learned:
- I learned that code can work for normal inputs but still fail on edge cases. JUnit testing helped me find the empty-array problem, and using AI through multiple iterations helped improve the solution.

Commit message:
- Iteration 3: final version passing all tests

---

## Final Reflection

What did you learn about using AI-generated code?
- I learned that AI-generated code can be a good starting point, but it is not always correct. The first AI-generated solution returned the sum instead of the largest value, and later testing showed that the empty array also needed to be handled.

How did testing help improve the program?
- Testing showed me exactly which inputs were causing problems. The JUnit tests helped guide each change until all four tests passed.

Why is iteration important when developing software?
- Iteration allows a programmer to make a change, test it, identify problems, and improve the code. Each iteration made the findResult method more accurate and reliable.

Would you trust AI-generated code without testing it? Why or why not?
- No. I would test AI-generated code before using it because the code may look correct but still fail certain requirements or edge cases.