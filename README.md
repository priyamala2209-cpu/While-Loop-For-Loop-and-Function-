# While Loop, For Loop and Fuctions

> Python Assignment 3 - Data Analytics (DA) Module 4

Loops are a fundamental concept in Python used to repeat a block of code multiple times. This project demonstrates the use of loops, control flow statements, and functions to solve simple real-world problems.

### Project Overview

This repository is part of the **Data Analytics (DA) - Module 4** Python assignment.

The objective of this assignment is to build a strong foundation in **loops, control statements, and functions in Python** through practical implementation.

This assignment contains 3 programs:

1.  **Number Guessing Game** - Implemented using `while` loop
2.  **Multiplication Table Generator** - Implemented using `for` loop
3.  **BMI Calculator** - Implemented using a user-defined `function`

All programs were developed and tested in **Jupyter Notebook**.

### Objectives

The main objectives of this assignment are:

* To understand and implement `while` loop for indefinite iteration
* To understand and implement `for` loop with `range()` function
* To understand control statements like `break`, `continue`, and `else`
* To create and use reusable Python functions
* To handle user input and output effectively
* To develop logical problem-solving skills
* To apply Python concepts to real-world use cases


## Tools and Technologies

* **Programming Language:** Python 3
* **Development Environment:** Jupyter Notebook
* **Core Concepts:** `while` Loop, `for` Loop, Functions, Control Flow Statements (`break`, `continue`, `else`)
* **Libraries Used:** `random` module

---

# Tasks Performed

## Task 1: Number Guessing Game (Using `while` Loop)

### Problem Statement
Develop an interactive Number Guessing Game using a `while` loop. The program generates a random number between **1 and 10**, and the user gets a maximum of **5 attempts** to guess the correct number. After each guess, the program provides feedback whether the guess is too high or too low.

### Concepts Used
* `while` loop for continuous attempts until win/loss condition
* `if`, `elif`, and `else` for logic and feedback
* `break` to exit the loop on correct guess
* `continue` to skip invalid inputs
* `random.randint()` to generate a random number
* `input()` for user interaction
* Conditional statements for game logic

  ### How It Works

1.  **Initialization:** The `random` module is imported and a secret number between 1 and 10 is generated using `random.randint(1, 10)`.
2.  **Attempt Setup:** The maximum number of attempts is set to 3.
3.  **Loop Execution:** A `while` loop runs until attempts are exhausted:
    - User is prompted to enter a guess.
    - **Input Validation:** If the guess is outside 1-10, a warning is shown and `continue` skips to the next iteration without counting it as a failed attempt.
    - **Comparison:** If the guess is higher than the secret number -> displays **"Too high. Try again."**
    - If the guess is lower than the secret number -> displays **"Too low. Try again."**
    - If the guess is correct -> displays a success message and `break` exits the loop.
4.  **Game Over Logic:** The `while-else` block executes only if the loop is not broken, displaying **"Better luck next time!"** when all attempts are used.

### Example Output

```text
Guess the number (between 1 and 10): 2
Too low. Try again.

Guess the number (between 1 and 10): 15
Your guess is out of range. Please guess a number between 1 and 10.

Guess the number (between 1 and 10): 5
Too high. Try again.

Guess the number (between 1 and 10): 3
Congratulations! You guessed the correct number.
```


## Task 2: Multiplication Table Generator (Using `for` Loop)

### Problem Statement
Develop a Python program that generates a multiplication table from **1 to 10** for a number entered by the user. This task demonstrates definite iteration using a `for` loop.

### Concepts Used
* `for` loop for definite iteration
* `range()` function to iterate from 1 to 10
* User input with `input()`
* Arithmetic operator (`*`) for multiplication
* Formatted output using f-strings

### How It Works

1.  **User Input:** The program takes an integer input from the user.
2.  **Iteration:** A `for` loop iterates through values from 1 to 10 using `range(1, 11)`.
3.  **Calculation:** In each iteration, the entered number is multiplied by the current loop counter (`i`).
4.  **Display:** The result is displayed in a clean, readable format:

```text
number x i = result
```

### Example

For the input `5`, the program produces:

```text
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50
```

## Task 3: BMI Calculator (Using Function)

### Problem Statement
A BMI (Body Mass Index) Calculator was developed using a user-defined Python function. The program calculates the Body Mass Index based on the user's weight and height and provides a health category.

### BMI Formula
```text
BMI = Weight (kg) / Height (m)²
```


### Concepts Used
* Function definition using `def`
* Function parameters and arguments
* `return` statement to return calculated value
* User input handling
* Arithmetic operations
* Formatted output with conditional logic

### Function Used

```python
def calculate_bmi(weight, height):
    return weight / (height ** 2)
```

### How It Works

1.  **Function Definition:** The `calculate_bmi()` function is defined to accept two parameters: `weight` and `height`.
2.  **User Input - Weight:** The user is prompted to enter their weight in kilograms.
3.  **User Input - Height:** The user is prompted to enter their height in meters.
4.  **Calculation:** The function calculates BMI using the formula: `Weight / (Height²)` and returns the value.
5.  **Result Display:** The returned BMI value is displayed rounded to two decimal places for better readability.

### Example Output

```text
Enter your weight in kg: 58
Enter your height in meters: 1.62

Your BMI is: 22.10
```

## Python Concepts Demonstrated

| Concept | Application in Project |
| :--- | :--- |
| **While Loop** | Used in the Number Guessing Game for repeated attempts |
| **For Loop** | Used to generate the Multiplication Table |
| **Range Function** | Used to iterate from 1 to 10 in the table generator |
| **Break Statement** | To exit the guessing loop when the correct answer is guessed |
| **Continue Statement** | To skip invalid guesses outside the range of 1-10 |
| **Else with Loop** | To display "Better luck next time" when attempts are exhausted |
| **Function** | Created `calculate_bmi()` for BMI calculation |
| **Parameters** | `weight` and `height` passed to the BMI function |
| **Return Statement** | Returning the calculated BMI value from the function |
| **Random Module** | Generating the secret random number using `random.randint()` |
| **User Input** | Taking values from the user via `input()` |
| **Conditional Statements** | `if-elif-else` logic for checking guesses and BMI categories |

# Project Structure

```text
Python-Assignment-3/
│
├── Python_Assignment_3.ipynb
│
└── README.md
```
### File Description

**Python_Assignment_3.ipynb**
Contains the complete implementation, execution, and output of all three tasks.

**README.md**
Contains the project overview, objectives, tools, task descriptions, concepts used, and project structure.

---

# Learning Outcomes

After completing this assignment, I gained practical knowledge of:

* Using `while` loops for repeated execution.
* Using `for` loops for iteration.
* Using `range()` to control loop iterations.
* Applying `break` and `continue` in loops.
* Understanding the `else` block with a `while` loop.
* Creating functions with parameters.
* Returning values from functions.
* Using Python's `random` module.
* Taking user input and displaying formatted output.
* Applying logical thinking to solve programming problems.

---

### Tech Stack

* Language: Python 3
* Environment: Jupyter Notebook
* Concepts: Loops, Conditional Statements, Functions

### How to Run

1. Clone the repository
2. Open the `.ipynb` file in Jupyter Notebook / VS Code
3. Run each cell to see the output

### Learning Outcomes

After completing this assignment, I gained hands-on experience in writing efficient loops, controlling program flow, and writing modular code using functions.

# Conclusion

This assignment provided practical experience with fundamental Python programming concepts. The **Number Guessing Game** helped demonstrate the use of a `while` loop and control statements such as `break`, `continue`, and `else`. The **Multiplication Table Generator** demonstrated the use of a `for` loop and the `range()` function. The **BMI Calculator** provided practice in creating functions, passing parameters, and returning calculated values.

Overall, these tasks strengthened my understanding of Python programming fundamentals and logical problem-solving skills, which are important for further learning in **Data Analytics and Python**.


Created By
--- 
Priyadharshini Naresh D
  ( Aspiring Data Analyst )
