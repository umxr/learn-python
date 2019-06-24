**Learning Python**

In your working directory, you need to make sure that you create a virtual environment.
Run this command to do so
`python3 -m vena env`

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
