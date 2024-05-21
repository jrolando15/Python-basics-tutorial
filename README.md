# Python-basics-tutorial
This tutorial covers the basics of Python programming language, including whitespace, importing modules, lists, tuples, dictionaries, functions, boolean expressions, and looping. It also includes a small homework activity at the end.

# Table of contents
# Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [importing Modules](#importing-modules)
- [List](#list)
- [Tuples](#tuples)
- [Dictionaries](#dictionaries)
- [Functions](#functions)
- [Boolean Expressions](#boolean-expressions)
- [Looping](#looping)
- [Homework](#homework)
- [License](#license)

# Installation
To run this tutorial, you need to have Python installed along with the following libraries:
- NumPy
You can install the required libraries using the following command
```bash
pip install numpy
```

# Usage
1. Clone the repository
```bash
git clone https://github.com/your_username/python-basics-tutorial.git
cd python-basics-tutorial
```

2. Run the Jupyter notebook
```bash
jupyter notebook
```

# Project Structure
```bash
python-basics-tutorial/
├── python_basics_tutorial.ipynb  # Jupyter notebook with the tutorial code
├── README.md                     # Project README file
└── requirements.txt              # List of dependencies
```
# Whitespace Is Important
In Python, whitespace (spaces and tabs) is significant and used to define code blocks. Here's an example:
```python
listOfNumbers = [1, 2, 3, 4, 5, 6]  # Create a list of numbers

for number in listOfNumbers:  # Iterate through the list
    print(number)  # Print the number
    if (number % 2 == 0):  # Check if the number is even
        print("is even")
    else:
        print("is odd")  # Print "is odd" if the number is odd

print("All done.")  # Print "All done" after the loop
```

# Importing Modules
Python modules can be imported and used in your code. Here's an example of importing the numpy module:
```python
import numpy as np  # Import the numpy module and alias it as 'np'

A = np.random.normal(25.0, 5.0, 10)  # Generate an array of 10 random numbers from a normal distribution
print(A)  # Print the array
```

# List
Lists are ordered collections of items. Here are some examples of working with lists:
```python
x = [1, 2, 3, 4, 5, 6]  # Create a list
print(len(x))  # Print the length of the list

print(x[:3])  # Print elements from the start up to (but not including) index 3
print(x[3:])  # Print elements from index 3 to the end
print(x[-2:])  # Print the last two elements

x.extend([7, 8])  # Extend the list with two more elements
print(x)

x.append(9)  # Append a single element to the end of the list
print(x)

y = [10, 11, 12]  # Create another list
listOfLists = [x, y]  # Create a list of lists
print(listOfLists)

print(y[1])  # Print the second element of the list 'y'

z = [3, 2, 1]  # Create a list
z.sort()  # Sort the list in ascending order
print(z)

z.sort(reverse=True)  # Sort the list in descending order
print(z)
```

# Tuples
Tuples are immutable (unchangeable) ordered collections of items. Here are some examples of working with tuples:
```python
x = (1, 2, 3)  # Create a tuple
print(len(x))  # Print the length of the tuple

y = (4, 5, 6)
print(y[2])  # Print the third element of the tuple 'y'

listOfTuples = [x, y]  # Create a list of tuples
print(listOfTuples)

(age, income) = "32,120000".split(',')  # Unpack values from a string
print(age)
print(income)
```

# Dictionaries
Dictionaries are unordered collections of key-value pairs. Here are some examples of working with dictionaries:
```python
captains = {}  # Create an empty dictionary
captains["Enterprise"] = "Kirk"
captains["Enterprise D"] = "Picard"
captains["Deep Space Nine"] = "Sisko"
captains["Voyager"] = "Janeway"

print(captains["Voyager"])  # Print the value associated with the key "Voyager"

print(captains.get("Enterprise"))  # Print the value associated with the key "Enterprise"
print(captains.get("NX-01"))  # Print None if the key is not found

for ship in captains:  # Iterate over the keys in the dictionary
    print(f"{ship}: {captains[ship]}")  # Print the key and its associated value
```

# Fucntions
Functions are reusable blocks of code that perform a specific task. Here are some examples of defining and using functions:
```python
def SquareIt(x):  # Define a function to square a number
    return x * x

print(SquareIt(2))  # Call the SquareIt function with the argument 2

def DoSomething(f, x):  # Define a function that takes another function as an argument
    return f(x)

print(DoSomething(SquareIt, 3))  # Call the DoSomething function with SquareIt and 3 as arguments

print(DoSomething(lambda x: x * x * x, 3))  # Use a lambda function as an argument
```

# Boolean Expressions
Boolean expressions evaluate to either True or False. Here are some examples of using boolean expressions:
```python
print(1 == 3)  # Print False (1 is not equal to 3)
print(True or False)  # Print True (using the or operator)
print(1 is 3)  # Print False (using the is operator for identity comparison)

if 1 is 3:  # Use an if-elif-else statement
    print("How did that happen?")
elif 1 > 3:
    print("Yikes")
else:
    print("All is well with the world")
```

# Looping 
Loops are used to iterate over a sequence (like a list or a string) or to repeat a block of code a specific number of times. Here are some examples of using loops:
```python
for x in range(10):  # Loop through the range from 0 to 9
    print(x)

for x in range(10):  # Loop through the range from 0 to 9
    if x == 1:  # Check if x is 1
        continue  # Skip the rest of the loop body and move to the next iteration
    if x > 5:  # Check if x is greater than 5
        break  # Exit the loop if x is greater than 5
    print(x)

x = 0  # Initialize x to 0
while x < 10:  # Loop as long as x is less than 10
    print(x)  # Print the current value of x
    x += 1  # Increment the value of x by 1
```

# Homework
Write some code that creates a list of integers, loops through each element of the list, and only prints out even numbers!


# License
This README file provides a comprehensive overview of your Python basics tutorial, including its description, installation instructions, usage, project structure, and detailed explanations of each topic covered. It also includes a homework activity to practice printing even numbers from a list.
