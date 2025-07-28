<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" class="logo" width="120"/>

# Rock Paper Scissors Game in Python

This README walks you through the [Rock_Paper_Scissors.ipynb](Rock_Paper_Scissors.ipynb) notebook, helping you understand how to play and how the code works—even if you’re just starting with Python or Jupyter notebooks!

## What Is This?

This notebook lets you play the classic “Rock, Paper, Scissors” game against the computer. You’ll pick one of the three—rock, paper, or scissors—and the computer will also make a choice. The notebook will then tell you who won.

## Code Explanation, Step by Step

### 1. Import the Random Module

```python
import random
```

- **What this does:** Brings in Python’s built-in `random` module, which allows the computer to make a random choice.
- **Beginner tip:** Modules are like toolboxes. `random` helps your programs do things randomly, like flipping a coin or, in this case, picking rock, paper, or scissors.


### 2. Set Up the Choices

```python
data = {'rock': 0, 'paper':1, 'scissors':2}
```

- **What this does:** Creates a dictionary named `data` to link the string names of choices (like 'rock') to numbers (0, 1, or 2).
    - rock → 0
    - paper → 1
    - scissors → 2
- **Why:** It helps the program turn words into numbers so they’re easier to compare in code.


### 3. Computer Makes Its Move

```python
computer_input = random.randint(0,2)
# print(computer_input)
```

- **What this does:** Asks the computer to pick a random number: 0, 1, or 2.
    - This is possible because `random.randint(a, b)` returns a number from **a** up to **b** (BOTH included).
- **Beginner tip:** Here, the computer can pick any of the three choices, thanks to the way `randint` works.


### 4. User Makes a Choice

```python
user_input = int(input('Choose 0 for rock, 1 for paper and 2 for scissors: '))
```

- **What this does:** Asks you (the user) to enter a number (0, 1, or 2) that matches your choice.
- **Beginner tip:** The text you type is turned into a number, so the program can compare it to the computer’s choice.


### 5. Figure Out Who Wins

```python
if user_input == computer_input:
    print('Draw')
elif (user_input == 0 and computer_input == 2) or \
     (user_input == 1 and computer_input == 0) or \
     (user_input == 2 and computer_input == 1):
    print('You win')
else:
    print('You lose')
```

- **What this does:**
    - If you and the computer pick the same number, it’s a draw.
    - If you pick the “winning” combination (like rock vs scissors), you win!
    - Otherwise, you lose.
- **How the rules work:**
    - Rock (0) beats scissors (2)
    - Paper (1) beats rock (0)
    - Scissors (2) beats paper (1)
- **Note:** `print` statements will tell you whether you won, lost, or got a draw.


## How To Play

1. **Open** the notebook (.ipynb) in Google Colab, Jupyter Notebook, or Jupyter Lab.
2. **Run each cell in order** (usually by clicking a play button at the top left of each cell, or pressing Shift + Enter).
3. **Enter your choice** when asked:
    - 0 for rock
    - 1 for paper
    - 2 for scissors
4. **See who wins!**

## What’s Good About This Version?

- The computer can pick any option (rock, paper, or scissors).
- The spelling for `'scissors'` is correct.
- The program tells you if you win, lose, or draw.


## Ideas to Improve

- Print out what both the user and the computer picked, so you can see both choices.
- Add a loop to play multiple rounds.
- Catch errors if you type something other than 0, 1, or 2.

Enjoy playing and experimenting!

---

<div style="text-align: center">⁂</div>

[^1]: Rock_Paper_Scissors-1.ipynb

