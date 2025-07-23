<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" class="logo" width="120"/>

# Day 2 Project: Tip Calculator

## Introduction

The **Tip Calculator** project is a beginner-friendly exercise designed to reinforce key Python concepts, including user input, arithmetic operations, type conversion, and string formatting. This program helps users accurately split a bill among several people, factoring in a user-chosen tip percentage—an everyday scenario ideal for practicing foundational coding skills.

## Problem Statement

Given a bill amount, a desired tip percentage, and the number of people splitting the bill, write a Python program that calculates and displays how much each person should pay. The program should:

- Display a welcome message.
- Prompt the user to enter:
    - The total bill amount.
    - The desired tip percentage (as a whole number, e.g., 10, 12, 15).
    - The number of people sharing the bill.
- Output the amount each person should pay, rounded to two decimal places for currency accuracy.


## Step-by-Step Solution

### 1. Greet the User

Begin by printing a welcome message to the user.

```python
print("Welcome to the tip calculator!")
```


### 2. Gather User Inputs

Ask for the necessary inputs and convert them to the appropriate types for calculations.

```python
bill = float(input("What was the total bill? $"))
tip = int(input("What percentage tip would you like to give? 10, 12, or 15? "))
people = int(input("How many people to split the bill? "))
```


### 3. Calculate the Total Bill Including Tip

Convert the tip percentage to a decimal, calculate the total bill with tip, and determine the amount per person.

```python
tip_as_percent = tip / 100
bill_with_tip = bill * (1 + tip_as_percent)
bill_per_person = bill_with_tip / people
final_amount = round(bill_per_person, 2)
```


### 4. Display the Result

Use string formatting to clearly present the final amount each person should pay.

```python
print(f"Each person should pay: ${final_amount}")
```


## Implementation Example

Here’s the complete program put together:

```python
print("Welcome to the tip calculator!")
bill = float(input("What was the total bill? $"))
tip = int(input("What percentage tip would you like to give? 10, 12, or 15? "))
people = int(input("How many people to split the bill? "))

tip_as_percent = tip / 100
bill_with_tip = bill * (1 + tip_as_percent)
bill_per_person = bill_with_tip / people
final_amount = round(bill_per_person, 2)

print(f"Each person should pay: ${final_amount}")
```


## Key Concepts Illustrated

| Concept | Example in Project |
| :-- | :-- |
| **Input Gathering** | `input()` function for user responses |
| **Type Conversion** | `float()` and `int()` to process numeric data |
| **Arithmetic** | Calculating tip and dividing total among people |
| **Rounding** | `round(value, 2)` to ensure results show two decimals |
| **Formatted Output** | `f-strings` for neat currency display |

## Usage Example

- User enters:
    - Total bill: `$124.56`
    - Tip: `12`
    - People: `7`
- Output:

```
Each person should pay: $19.93
```


## Troubleshooting \& Tips

- Always convert user input to the correct numeric type before calculations.
- Ensure tip percentages are whole numbers and no `%` symbol is included.
- Remember rounding to two decimal places is important for currency accuracy.
- Customize the prompts or extend functionality (e.g., allow custom tip values, input validation) as additional practice.


## Conclusion

This project demonstrates how basic Python features come together to solve a practical problem. By working through this exercise, you build confidence in handling user input, performing calculations, and presenting results—the foundation for many future coding challenges.

**Feel free to download and customize this README for your own GitHub project, and keep experimenting with your Tip Calculator to learn more!**

<div style="text-align: center">⁂</div>

[^1]: Untitled0.ipynb

