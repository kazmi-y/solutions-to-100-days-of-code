Day 1 Project: Band Name Generator
Introduction to the Band Name Generator Project
In this final project, we will build a Band Name Generator program. The program asks the user for the city they grew up in and the name of their pet, then combines these inputs to create a band name.

You can check out the project by visiting the provided link or by navigating to the Course Resources page and clicking the corresponding link. The program's interface prompts the user for input and then displays the generated band name.

User Input and Cursor Formatting
Notice that when the input prompt appears, the cursor shows up on a new line. For example, when the program asks, "What's the name of the city you grew up in?", the cursor appears on the following line, providing a clean input interface.

Project Instructions
You are encouraged to complete this project by applying everything learned so far, including printing, input handling, variables, new lines, string manipulation, and debugging. Once completed, your program should function identically to the example provided.

Take a moment to prepare yourself, then pause the video and tackle this final project.

Solution Walkthrough
If you have completed the project or want to verify your solution, continue watching for a detailed walkthrough of the implementation.

Step 1: Greeting Message
Start by creating a greeting message for the program. For example, print "Welcome to the Band Name Generator." using the print() function.

python Code Sample
print("Welcome to the Band Name Generator.")
Step 2: Prompt for City Name
Next, ask the user for the city they grew up in using the input() function with a prompt string. Store the user's response in a variable named city.

python Code Sample
city = input("Which city did you grow up in?\n")
Step 3: Prompt for Pet Name
Similarly, ask the user for the name of a pet and store the response in a variable named pet.

python Code Sample
pet = input("What is the name of a pet?\n")
Step 4: Combine Inputs to Generate Band Name
Use string concatenation to combine the city and pet names with a space in between. Then, print the resulting band name with an introductory message.

python Code Sample
print("Your band name could be: " + city + " " + pet)
Step 5: Formatting Input Prompts
To ensure the input cursor appears on a new line after the prompt, add a newline character (\n) at the end of each input prompt string. This improves the program's readability and user experience.

Conclusion
This completes the Band Name Generator project. You have applied fundamental Python concepts such as printing, input handling, variables, string concatenation, and formatting to create a functional and user-friendly program.

Tomorrow, more tutorials, code challenges, and projects await to deepen your Python knowledge. Rest well and let your brain process today's learning. See you tomorrow!

Key Takeaways
Created a Band Name Generator that combines user inputs to generate a band name.
Used the input() function to capture user responses and stored them in variables.
Applied string concatenation and newline characters (\n) to format output and input prompts.
Enhanced user experience by positioning the input cursor on a new line after prompts.
