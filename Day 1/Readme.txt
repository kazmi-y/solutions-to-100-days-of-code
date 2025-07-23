<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" class="logo" width="120"/>

# Day 1 Project: Brand Name Generator

## Introduction to the Brand Name Generator Project

This project is designed as a beginner-friendly exercise to practice Python fundamentals, user input handling, and string formatting. The program creates a fun "Brand Name Generator" by asking the user for the city they grew up in and their pet’s name, then combines these inputs to form a unique brand name.

The code follows a simple, interactive flow:

- It greets the user
- Requests user input for two questions
- Combines and outputs the result as a potential brand name


## Program Instructions

You are encouraged to follow each step carefully and ensure the final program behaves as intended. The project covers essential Python skills:

- Printing output
- Capturing and storing user input
- String manipulation and formatting
- Debugging


### Step-by-Step Solution

#### Step 1: Greeting Message

Start by displaying a welcome message to the user.

```python
greeting = "Welcome to the Brand Name Generator"
print(greeting)
```


#### Step 2: Prompt for City Name

Ask the user to input the city where they grew up. Store the response in a variable.

```python
query1 = "Which city did you grew up in?"
print(query1)
userinput = input("Enter City name: ")
```


#### Step 3: Prompt for Pet Name

Prompt the user for the name of their pet, and store the response.

```python
query2 = "What is the name of your pet?"
print(query2)
userinput2 = input("Enter Pet name: ")
```


#### Step 4: Generate and Display Brand Name

Combine the two inputs using string formatting to generate and display the brand name.

```python
print(f"Your band name is {userinput} {userinput2}")
```


## Enhancing User Experience

- Adding a newline character (`\n`) in input prompts can position the cursor on the next line, improving readability.
- Keep prompts clear, concise, and user-friendly.


## Summary Table

| Feature | Implementation Example |
| :-- | :-- |
| Greeting the user | `print("Welcome to the Brand Name Generator")` |
| Asking for city name | `input("Enter City name: ")` |
| Asking for pet name | `input("Enter Pet name: ")` |
| Showing the generated result | `print(f"Your band name is ...")` |

## Conclusion

This project demonstrates foundational Python programming concepts, including user input, variable assignment, and string formatting, in a fun and engaging way. By following these steps, you can easily build your own interactive Brand Name Generator.

Take some time to experiment with different input prompts and output formats to further enhance the project!

<div style="text-align: center">⁂</div>

[^1]: Brand_name_generator.ipynb

[^2]: Readme.txt


