# Functions

It is a block of code which executes only when it is called.

They are a handy way to creating blocks of code that you can reuse.

To define a function, you use the *def* keyword, followed by *function_name*, parentheses then the body of the function.

a function can one or more arguments.

**parameter vs argument**

a parameter is the variable listed inside the parentheses when defining a function.

an argument is the literal value passed to a function, when calling it for execution

![image](https://github.com/MisterWest11/Python-Week-1-4/assets/152319557/b4e6bbf9-8766-4a5c-9b0b-80ae0ca6f23f)

**Lambda Functions**

A Python function that has only one expression and can't have multiple lines. It is meant to make it easier to create some small logic in one line instead of a whole function.

They are anonymous, meaning there is no need to name them.

*Basic Syntax*

use the *lambda* keyword, define parameters needed, use : to separate parameters from the expression

*lambda arguments: expression*

this example below is a lambda function with one parameter

![image](https://github.com/MisterWest11/Python-Week-1-4/assets/152319557/3bc76eff-6715-4192-b5fc-17c5b9f2730d)



multiple parameter 

![image](https://github.com/MisterWest11/Python-Week-1-4/assets/152319557/d48dcd9a-9a96-41b3-b0ac-bfecd3ea5676)


**Map function**

- applies a function to each item in an iterable (list, tuple, set or dictionary).

map(function, iterable)


**Filter() function**

Creates a collection of elements from an iterable for which a function returns

![image](https://github.com/MisterWest11/Python-Week-1-4/assets/152319557/ac01a729-70e1-4493-a8d5-57d27f1e0638)


# Scope

in Python, there are two types of variables, Local variables which are defined inside the function. Global variables are defined outside the function in the main block.

**Locals()**

Variables defined within the scope of a function, are only accessible to the function and not anywhere outside the function.

**Global**

Variables defined in the main method, not within a function. used anywhere throughout the program.


# Classes & Objects

A class in a blueprint or real world representation of an object.
It contains attributes and method the class can possess. 

We have instance variables that contain data that is unique to each instance(object).

when creating a Class, we get a default function known as an *__init__()* function (constructor) which initializes an instance upon creation.

**Class Attributes and Methods**

Instance attributes are properties found in a class. 

Instance variables: attributes attached to an instance of a class. We define instance variables in the constructor ( the __init__() method of a class).

Class Variables: a variable that is declared inside a class.

Instance Methods: Used to access or modify the instance attributes.

![image](https://github.com/MisterWest11/Python-Week-1-4/assets/152319557/4d94b5d7-91e8-4207-b15b-8a1e5637a6d3)


# Inheritance

When a subclass inherits attributes and functionalities of a parent class.

Class Methods: Used to access or modify the class state.

Static Methods: a method that performs a task in isolation. They don't have access to class attributes.

![image](https://github.com/MisterWest11/Python-Week-1-4/assets/152319557/e204c849-47a9-495e-895e-daf066585e2e)



# Exceptions

An error event that interrupts the flow of the program.

use a try-except method. in the *try* block, we have the code that is more likely to create an error in a program. in the *except* block, we handle our error in a smarter way, to help counter an interruption in our program flow.


![image](https://github.com/MisterWest11/Python-Week-1-4/assets/152319557/bd7baf24-e6b9-4c9c-9f04-f274b9abcf8a)

We also have the *finally* block that executes no matter an exception was found or not.


# Fundamentals of Threads and Processes

A Thread is a flow of execution. basically a seperate of instructions that run on different processors in the computer only 1 ata time in python.

a process is an instance of a program. it has memory set aside for its code and data.
a process can get multiple threads and execute code at the same time in parallel.


# File Handling

The key function for working with files in Python is using the open() function. The open() function takes two paramteres: *filename & mode*

there are four different methods for opening a file:

* "r" - Read - Opens a file for reading, error if the file does not exist.

* "a" - Append - Opens a file for appending, creates the file if it does not exist.

* "w" - Write - Opens a file for writing, creates a file if it does not exists

* "x" - Create - creates a specified file, returns error if it does not exist.


**To open a file for reading:**

   f = open("demofile.txt")

Read Only Parts Of The File

read() method returns the whole text, but you can also specify how many characters to return.

**Write to an existing file**

* "a" - Append - will append to the end of the file.

* "w" - Write - will overwrite any existing content.

  ![image](https://github.com/MisterWest11/Python-Week-1-4/assets/152319557/81db2da0-ab43-43cb-85e9-3af5538f7e6c)


**Create a new File**

* "x" - Create - will create a new file, return error if it does not exist.

* "a" - Append - will create a file if the specified file does not exist.

* "w" - Write - will create a file if the specified file does not exist.

**Delete a file**

To delete a fil, you must import the OS module and run its os.remove() function.

to check if a file exists:

![image](https://github.com/MisterWest11/Python-Week-1-4/assets/152319557/9233d1db-348f-4cc1-9ee0-43b51ffcb37e)

# JSON Files

Python has a built-in package called json, used to work with *json* data.

  **import json**

*Convert from JSON to Python*

you can parse it using the json.loads() method, the result is a Python Dictionary.

![img.png](img.png)

if you want to convert from Python to JSON

if you have a Python object, you can convert it to a JSON string by using the json.dumps() method.

![img_3.png](img_3.png)

You can convert Python objects of the following types into JSON strings:

* dict
* list
* tuple
* string
* int
* float
* True
* False
* None


