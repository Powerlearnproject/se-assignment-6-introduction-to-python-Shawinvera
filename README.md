[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15343850&assignment_repo_type=AssignmentRepo)

# SE-Assignment-6

Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

Questions:

1. Python Basics:

   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
     Python is a high-level, interpreted programming language known for its simplicity, readability, and versatility
     Simplicity and Readability: Python's syntax is clear, concise, and easy to learn, making it accessible for beginners and experienced developers alike. Its indentation-based block structure promotes clean and readable code.
     Versatility: Python supports multiple programming paradigms, including procedural, object-oriented, and functional programming styles. It can be used for a wide range of applications, from web development to scientific computing and data analysis.
     Extensive Standard Library: Python comes with a large standard library that provides modules and packages for tasks such as file I/O, networking, regular expressions, and more. This reduces the need for developers to write code from scratch for common tasks.

2. Installing Python:

   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
     Download Python Installer:

Visit the official Python website at https://www.python.org/downloads/.
Download the latest version of Python for Windows (usually displayed prominently on the page).
Choose the installer based on your system architecture (32-bit or 64-bit).
Run the Installer:

Once downloaded, run the Python installer (typically named something like python-3.x.x.exe).
Make sure to check the option "Add Python X.X to PATH" during the installation process. This step is important for Python to be accessible from the command line.
Verify Installation:

Open a command prompt (cmd) and type python --version or python3 --version.
You should see the installed Python version printed out if the installation was successful.
Create a Virtual Environment:

Navigate to your project directory in the terminal.
Create a virtual environment named env (or any name you prefer) by running:
python -m venv env
Activate the Virtual Environment:

Activate the virtual environment:
On Windows (cmd):
.\env\Scripts\activate
Verify Activation:

Your command prompt should now be prefixed with (env) to indicate the virtual environment is active.

While the virtual environment is active, install Python packages using pip as usual
pip install package_name
Deactivate the Virtual Environment:
To exit the virtual environment, simply type:
deactivate

3. Python Syntax and Semantics:

   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
     print("Hello, World!")
     Print Statement (print()):
     The print() function in Python is used to output data to the console (standard output). It takes zero or more arguments inside parentheses and prints them as text.
     In the example, print("Hello, World!") prints the string "Hello, World!" to the console.
     tring Literal ("Hello, World!"):

A string literal in Python is a sequence of characters enclosed within double quotes ("). Strings are used to represent text and are a fundamental data type in Python.
In the program, "Hello, World!" is a string literal that represents the text we want to output.

4. Data Types and Variables:

   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
     Integer (int):
     Represents whole numbers without any decimal point.
     Example: 42, -10, 0.
     Float (float):
     Represents numbers with a decimal point.
     Example: 3.14, -0.001, 2.0.
     String (str):
     Tuple (tuple):
     Similar to lists, but they are immutable (cannot be changed after creation).
     Example: (1, 2, 3), ('apple', 'banana', )
     Represents sequences of characters enclosed in single (') or double (") quotes.
     Example: 'Hello', "Python", '123'. # Define variables of different data types
     integer_var = 42
     float_var = 3.14
     string_var = 'Hello, Python!'
     boolean_var = True
     list_var = [1, 2, 3, 4, 5]
     tuple_var = ('apple', 'banana', 'cherry')
     dictionary_var = {'name': 'Alice', 'age': 30, 'city': 'New York'}

# Print out the variables and their types

print(f'Integer Variable: {integer_var}, Type: {type(integer_var)}')
print(f'Float Variable: {float_var}, Type: {type(float_var)}')
print(f'String Variable: {string_var}, Type: {type(string_var)}')
print(f'Boolean Variable: {boolean_var}, Type: {type(boolean_var)}')
print(f'List Variable: {list_var}, Type: {type(list_var)}')
print(f'Tuple Variable: {tuple_var}, Type: {type(tuple_var)}')
print(f'Dictionary Variable: {dictionary_var}, Type: {type(dictionary_var)}')

5. Control Structures:

   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
     Conditional Statements (if-else statement):
     Conditional statements are used to execute specific blocks of code based on whether a certain condition is True or False. # Example of an if-else statement
     x = 10

if x > 0:
print(f'{x} is positive.')
else:
print(f'{x} is not positive.')
Loops (for loop):
Loops are used to repeat a block of code multiple times until a certain condition is met or for a specified number of iterations.

Example of a for loop:

# Example of a for loop

fruits = ['apple', 'banana', 'cherry']

for fruit in fruits:
print(fruit)

6. Functions in Python:

   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
     In Python, functions are blocks of code that are designed to perform a specific task. They allow you to encapsulate reusable code and execute it multiple times without rewriting the same code.
     Importance of functions
     Code Reusability: Functions allow you to define a block of code once and use it multiple times throughout your program.
     Modularity: Functions promote modular programming by breaking down large tasks into smaller, manageable pieces.
     Abstraction: Functions abstract away the implementation details, making the code more readable and easier to maintain.
     def add_numbers(a, b):
     """Function to add two numbers."""
     return a + b

# Calling the function with arguments 3 and 5

result = add_numbers(3, 5)
print(f"The sum of 3 and 5 is: {result}") # Output: The sum of 3 and 5 is: 8

# Calling the function with arguments -10 and 20

result = add_numbers(-10, 20)
print(f"The sum of -10 and 20 is: {result}") # Output: The sum of -10 and 20 is: 10

7. Lists and Dictionaries:

   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
     Lists: Lists are ordered collections of items, where each item is indexed by its position.
     Characteristics:
     Elements are stored in a sequence.
     Elements can be accessed by their index.
     Lists are mutable, meaning you can modify elements in place.
     Lists allow duplicate elements.
     Syntax: Lists are defined using square brackets [].
     Dictionaries:Purpose: Dictionaries are unordered collections of key-value pairs.
     Characteristics:
     Elements are stored as key-value pairs.
     Elements are accessed by their keys rather than by index.
     Dictionaries are mutable.
     Keys must be unique and immutable (strings, numbers, tuples), but values can be mutable and can be duplicated.
     Syntax: Dictionaries are defined using curly braces {}, with key-value pairs separated by colons :. # Create a list of numbers
     numbers = [1, 2, 3, 4, 5]

# Create a dictionary of key-value pairs

person = {
'name': 'Alice',
'age': 30,
'city': 'New York',
'email': 'alice@example.com'
}

# Print the list and dictionary

print("List of numbers:", numbers)
print("Dictionary of person:", person)
print()

# Accessing elements:

print("Accessing elements:")
print("First number in the list:", numbers[0])
print("Age of the person:", person['age'])
print()

# Modifying elements:

print("Modifying elements:")
numbers[2] = 10
person['city'] = 'San Francisco'
print("Updated list of numbers:", numbers)
print("Updated dictionary of person:", person)
print()

# Adding elements:

print("Adding elements:")
numbers.append(6)
person['phone'] = '123-456-7890'
print("List after adding 6:", numbers)
print("Dictionary after adding phone number:", person)
print()

# Removing elements:

print("Removing elements:")
removed_number = numbers.pop(2)
del person['email']
print("Removed number from list:", removed_number)
print("Dictionary after deleting email:", person)
print()

# Length of list and dictionary:

print("Length of list:", len(numbers))
print("Number of keys in dictionary:", len(person))

8. Exception Handling:

   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
     Exception handling in Python allows you to manage and respond to errors that occur during program execution gracefully. # Example function that divides two numbers
     def divide_numbers(a, b):
     try:
     result = a / b # Attempt division
     except ZeroDivisionError:
     print("Error: Division by zero!")
     except TypeError as e:
     print(f"Error: {e}")
     else:
     print(f"{a} divided by {b} is equal to {result}")
     finally:
     print("Division operation completed.\n")

9. Modules and Packages:

   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
     Modules:
     A module in Python is a single file containing Python code that defines functions, classes, and variables. It allows you to logically organize your Python code for better readability and reusability. Modules are imported into other Python scripts to make use of their defined functions, classes, or variables.
     Packages:
     A package in Python is a directory of Python modules containing an additional **init**.py file. This file indicates that the directory is a Python package and allows for hierarchical structuring of the module namespace. Packages help in organizing and managing multiple modules under a common namespace.

# Example: Using the math module to calculate the square root

# Importing the math module

import math

# Using a function from the math module

num = 16
square_root = math.sqrt(num)

# Printing the result

print(f"The square root of {num} is {square_root}")

10. File I/O: - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    Reading from a File:
    To read from a file in Python, you typically follow these steps:

Open the File: Use the open() function to open a file in read mode ('r'). It returns a file object.
Read Content: Use methods like read(), readline(), or readlines() to read the content of the file.
Close the File: Always close the file using the close() method to free up system resources.

# Example: Reading from a file and printing its content

# Open the file in read mode

file_path = 'sample.txt' # Replace with your file path
try:
with open(file_path, 'r') as file:
content = file.read() # Read the entire content of the file
print(content) # Print the content to the console
except FileNotFoundError:
print(f"Error: The file '{file_path}' was not found.")
except IOError as e:
print(f"Error: {e}")

Writing to a File:
To write to a file in Python, you generally follow these steps:

Open the File: Use the open() function with write mode ('w') or append mode ('a'). Write mode ('w') overwrites the file if it exists, while append mode ('a') appends to the end of the file if it exists or creates a new file.
Write Content: Use the write() method to write data to the file. You can write strings or iterate over lines of data to write multiple lines.
Close the File: Always close the file after writing to ensure all data is flushed to disk and resources are released.

# Example: Writing a list of strings to a file

# List of strings to write to the file

lines_to_write = [
"First line of text\n",
"Second line of text\n",
"Third line of text\n"
]

# File path where we want to write

output_file = 'output.txt' # Replace with your file path

try: # Open the file in write mode ('w')
with open(output_file, 'w') as file: # Write each line from the list to the file
for line in lines_to_write:
file.write(line)
print(f"Successfully wrote {len(lines_to_write)} lines to {output_file}")
except IOError as e:
print(f"Error writing to file: {e}")

# Submission Guidelines:

- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].
