<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" class="logo" width="120"/>

# Treasure Island: Adventure Game

## Problem Overview

**"Treasure Island"** is a text-based adventure game. The goal is to lead the player through a series of choices, each affecting the journey to find a hidden treasure. The game tests logical reasoning, handling of conditional statements, and user interaction in Python.

### Game Story

- The player begins at the entrance to Treasure Island.
- At each stage, they are prompted to make a decision, and their choices determine whether they advance, win, or face a "Game Over" scenario.
- The outcome is decided strictly by following the flow defined in the code and the provided flowchart.


## Game Flow Summary

### 1. Greeting and Introduction

The game starts by displaying welcoming ASCII art (from `logo.py`) and a message introducing the mission.

### 2. First Choice: The Crossroad

- Prompt: “You are at a cross. Where do you want to go? type 'left' or 'right'”
- **left** → proceed to the lake.
- **right** (or any other input) → fall into a hole. Game Over.


### 3. Second Choice: The Lake

- Prompt (after choosing left): “You've come to a lake... Type 'wait' to wait for a boat. Type 'swim' to swim across.”
- **wait** → arrive at the island.
- **swim** (or any other input) → attacked by trout. Game Over.


### 4. Third Choice: The Doors

- Prompt: “There is a house with 3 doors. One red, one yellow, and one blue. Which colour do you choose?”
    - **yellow** → You found the treasure! You Win!
    - **red** → It's a room full of fire. Game Over.
    - **blue** → You enter a room of beasts. Game Over.
    - Any other input → Game Over.


## Solution: Step-by-Step Code Walkthrough

Below is the exact logic and structure implemented in `Treasure_Island.ipynb`:

```python
# Display ASCII art from file (logo.py)
logo = '/content/logo.py'
with open(logo, 'r') as f:
    file_content = f.read()
    print(file_content)

# Greeting and instructions
print("Welcome to the treseure Island \nYour mission is to find the Treasure ")

# First decision point
print("You are at a cross. Where do you want to go?\ntype 'left' or 'right'")
input_1 = input("Choose left or right: ")

if input_1 == "left":
    # Second decision point
    input_2 = input(
        "You've come to a lake. There is an island in the middle of the lake. "
        "Type 'wait' to wait for a boat. Type 'swim' to swim across. : "
    )
    if input_2 == "wait":
        # Third decision point
        input_3 = input(
            "You arrive at the island. There is a house with 3 doors. "
            "One red, one yellow and one blue. Which colour do you choose? : "
        )
        if input_3 == "yellow":
            print("You found the treasure! You Win!")
        elif input_3 == "red":
            print("It's a room full of fire. Game Over.")
        elif input_3 == "blue":
            print("You enter a room of beasts. Game Over.")
        else:
            print("Game over.")
    else:
        print("You got attacked by an angry trout. Game Over")
else:
    print("You fell into a hole. Game Over.")
```


## Flowchart Reference

- All decisions ("left" vs "right", "wait" vs "swim", door colors) directly map to code logic above.
- Game ends as soon as the player makes an incorrect choice at any stage.


## Key Programming Concepts Demonstrated

| Concept | Example in This Project |
| :-- | :-- |
| User Input | `input()` |
| Conditional Logic | `if/elif/else` |
| String Output | `print()` |
| File Handling | Reading/displaying ASCII art from file |
| Nested Conditionals | Structure of multiple decision points |

## Typical Game Run Example

```
Welcome to the treseure Island 
Your mission is to find the Treasure 
You are at a cross. Where do you want to go?
type 'left' or 'right'
Choose left or right: left
You've come to a lake. There is an island in the middle of the lake. Type 'wait' to wait for a boat. Type 'swim' to swim across. : wait
You arrive at the island. There is a house with 3 doors. One red, one yellow and one blue. Which colour do you choose? : yellow
You found the treasure! You Win!
```


## Conclusion

This project demonstrates how to build an interactive, text-based adventure using Python's basic features. Through user input, print statements, and conditional checks, players can experience different outcomes, learning valuable programming and logic skills along the way.

Try altering the messages, adding new decision points, or expanding the story as exercises to improve your control flow and creative thinking.

<div style="text-align: center">⁂</div>

[^1]: Treasure_Island.ipynb

[^2]: Treasure-Island-Flowchart-pdf.pdf

