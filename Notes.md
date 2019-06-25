**Learning Python**

In your working directory, you need to make sure that you create a virtual environment.
Run this command to do so
`python3 -m venv env`

To instantiate the environment, run the following command
`source env/bin/activate`

This must be run prior to working in the director. You’ll know if the environment is running by noticing an ‘env’ prefix in your terminal

**Helpful methods:**

- type(param) => returns the type of the param
- dir(param) => returns all the methods available on the param
- print(param) => prints the param to the console
- help(param) => lists helpful information about that param

**Variables**

- Should be lowercase
- If its more than one word, then separate each word with an underscore

**Numbers**

- Basically the same as JS
- float(param) => returns floating point number
- int(param) => returns integer
- str(param) => returns string

**Strings**

- Best practice to use double quotes
- Similar to JS
- “”” … … … “” => long string. When using the REPL, … Is basically adding a new line of information. You need to close with “”” for the long string to end
- F”Hello, {variable}” => basically the same as template strings in js.


**Functions**

- def name() => defines a function called name
- In python we dont use brackets to show function block, instead we use indentation

Basic function examples:

`
def print_first_name(name):
  print(f"Hello {name})
`

`
def my_age(age):
  return 22`
`

`
def add_numbers(a,b):
  return a + b
`

`
def greeting(name):
  greeting = "Hello "
  return greeting + name
`

**Function Arguements**

- function arguements can have fallback defaul arguements. default arguements always come after those that are required
- if a functions arguemnts all have fallback, they can be passed in any order as you want. the reason being is that they are labelled
- 

default arguement examples

`
def gretting(name, greeting="Hello"):
  print(f"{greeting}, {name})
`


`
def foo(a, b=10):
  return a + b
`
the following function calls return the same value, just a slightly different way to call them. 
Both of them will return 3.

` foo(1, b=2) `
` foo(1, 2) `