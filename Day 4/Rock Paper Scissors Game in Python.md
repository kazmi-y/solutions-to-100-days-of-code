<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" class="logo" width="120"/>

# Rock Paper Scissors Game in Python

This README explains how the provided [Rock_Paper_Scissors.ipynb](Rock_Paper_Scissors.ipynb) notebook builds a simple Rock, Paper, Scissors game using Python and NumPy. If you're new to programming or Jupyter Notebooks, don’t worry—this will walk you through each cell, step by step.

## What Is This?

It's a classic "Rock, Paper, Scissors" game that you play against the computer in your notebook! You choose either rock, paper, or scissors, and so does the computer (randomly). The game then tells you who won.

## Code Walkthrough

Below is an explanation of what each code cell in the notebook does, in order:

### **1. Importing NumPy**

```python
import numpy as np
```

- **What it does:** Brings in the NumPy library, which allows us to generate random numbers (needed for the computer’s move).
- **If you’re new:** NumPy is a popular library in Python for handling arrays and random number generation and is commonly used in many games and data science projects.


### **2. Defining Choices**

```python
data = {'rock': 0, 'paper':1, 'Sissors':2}
```

- **What it does:** Sets up a dictionary linking each word (“rock”, “paper”, “Sissors”) to a number.
    - `rock` = 0
    - `paper` = 1
    - `Sissors` = 2
- **If you’re new:** Dictionaries like this help us translate between numbers and names.


### **3. Computer Chooses Randomly**

```python
computer_input = np.random.randint(0,2)
```

- **What it does:** Makes the computer pick a random number: **0** or **1** (but not including **2**).
- **Note:** This means the computer only ever picks between "rock" (0) or "paper" (1), not "Sissors" (2). This is an error; usually, you want to use `np.random.randint(0,3)` to include all three possibilities.
- **If you’re new:** `np.random.randint(a, b)` generates a random integer from `a` (inclusive) to `b` (exclusive).


### **4. Ask the User for a Choice**

```python
user_input = int(input('Choose 0 for rock, 1 for paper and 2 for scissors: '))
```

- **What it does:** Asks the user to type in a number representing their move:
    - 0 = Rock
    - 1 = Paper
    - 2 = Scissors
- **If you’re new:** The `input()` function gets input as text, and `int()` converts that text to a number.


### **5. Determining the Winner**

```python
if user_input == computer_input:
    print('Draw')
elif (user_input == 0 and computer_input == 2) or \
     (user_input == 1 and computer_input == 0) or \
     (user_input == 2 and computer_input == 1):
    print('You win')
else:
    print('You loose')
```

- **What it does:**
    - If both you and the computer pick the same thing, it prints **Draw**.
    - Else, it checks if your combination beats the computer:
        - **Rock (0) beats Scissors (2)**
        - **Paper (1) beats Rock (0)**
        - **Scissors (2) beats Paper (1)**
    - If you win, it prints **You win**, otherwise **You loose** (typo: should be "lose", but it says "loose" in the notebook).
- **If you’re new:** The backslash (`\`) is for breaking up a long logical line over two lines.


## How To Run

1. **Open the .ipynb file** in Google Colab, Jupyter Notebook, or Jupyter Lab.
2. **Run the cells one by one.**
3. **When prompted**, choose a number (0/1/2) and see if you beat the computer!


Enjoy coding and playing! If you’re new, try making small changes and rerunning—it's a great way to learn.

<div style="text-align: center">⁂</div>

[^1]: Rock_Paper_Scissors.ipynb

