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

`def print_first_name(name): print(f"Hello {name})`

`def my_age(age): return 22`
`

`def add_numbers(a,b): return a + b`

`def greeting(name): greeting = "Hello " return greeting + name`

**Function Arguements**

- function arguements can have fallback defaul arguements. default arguements always come after those that are required
- if a functions arguemnts all have fallback, they can be passed in any order as you want. the reason being is that they are labelled
-

default arguement examples

`def gretting(name, greeting="Hello"): print(f"{greeting}, {name})`

`def foo(a, b=10): return a + b`

the following function calls return the same value, just a slightly different way to call them.
Both of them will return 3.

`foo(1, b=2)`
`foo(1, 2)`

**Function Examples**

`def add_numbers(a,b): return a + b`

`def greeting(name, greeting="Hello"): print(f"{greeting}, {name}")`

**Lists**

These are pretty much the equivalent of arrays in js
retain the order of the items in the list
bracket notation can be used to access items in the array similar to javascript
trying to access an item at an index which doesnt exist will return an index error
bracket notation is used to update an item. the only difference is that assignment is used once you have chosen the index

- `[1]`
- `list(1)`
- `["person 1", "person 2"]`

**Methods**

- len() => takes in a param and returns the length of the parameter
- sorted() => takes in a param and returns a sorted version of the array without effecting the param. the returned value is a clone of the param. the sorted command also takes in a second parameter which allows you to reverse the order of the list.
- [arr].sort() => modifies the original array and sorts the array
- [arr].reverse() => modifies the original array and reverses the array.
- [arr].append(param) => appends the past parameter to the array
- [arr].insert(pos,item) => adds an item to the specified position in an array
- [arr1].extend([param]) => concatenates the array param to the original array. modifies the original array
- "str" in [arr] => returns a boolean depending on if the "str" is in the array
- [arr].index(param) => returns the index of the param
- [arr].count(param) => counts upto the passed param in the array and returns the index
- [arr].remove(param) => removes the passed param from the array. if there are duplicate values. the remove method will only remove the first instance of it. if you try to remove an element that doesnt exist in the array, you will get a value error instead of an index error
- [arr].pop() => removes the last element in the array and returns the element that was just removed
- [arr].pop(index) => remove the item in the passed index and returns the element that was just removed - trying to remove an element at an index which doesnt exist will give you an index error

**Common Gotchas**

- creating a list with a missing comma will result in a syntax error
- forgetting to close a list will also result in a syntax error

**Tuples**

tuples are a lightweight collection of related items. tuples are immutable. once the tuple has been created, the items cannot be changed. useful for things like containing a snapshot of data.

`a = () => creates a tuple and is assigned to 'a'`

ways of creating a tuple:

`a = 1,2`
`a = (1,2)`

- tuple items can be accessed the same way you try to access lists. (bracket notation)
- trying to mutate an item in the tuple will return a type error

**Unpacking**

this is basically the same as js destructuring

`me = ("umar",22,"developer)`
`name, age, job = me`

if the number of unpacked variables dont match the number of items in the tuples. you will get a value error.
if you want to ignore a certain value when unpacking, be sure to use the `_` instead of passing a variable name

**Sets**

a collection a data that allows you to store other data types which are immutable and is unordered. you wont be able to reference data stored in a set like arrays or tuples. searching for items in sets is a very fast operation. `set()` will create an empty set. Sets cannot have duplicate values. if you create a set with a duplicate value (Case sensitive), they will automatically get removed during compile time. sets can contain other data types like string, int, float, lists etc. trying to access an item in the set using bracket notation will results in a type error.

**Methods**

- len(param) => returns the length of the set
- my_set.add(param) => will add the param to the set
- my_set.discard(param) => will discard the param from the set. if you try to discard an item that no longer exists in the set, nothing will happen. no error, nothing
- my_set.remove(param) => will remove the param from the set. if you try to remove an item that no longer exists in the set, you will get a key error
- my_set.update(my_second_set) => will combine the two sets together. the update function expects a sequence, if you were to pass a string, you'll notice that the string is split up into a list of its individual characters.

**Operations**

you can use the in keyword to check if an item exists in your set

`colours = {"Red", "Green". "Blue"}`
`"Red" in colours => returns True`
`"Orange in colours => returns False"`

- Union => Merges set_1 and set_2 making sure to remove any duplicates
- Intersection => Merges set_1 and set_2 with only items that appear in both sets
- Difference => Merges set_1 and set_2 with only items that dont appear in both sets
