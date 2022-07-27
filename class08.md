# List Comprehensions

Python list comprehension consists of brackets containing the expression, which is executed for each element along with the for loop to iterate over each element in the Python list. List comprehension offers a shorter syntax when you want to create a new list based on the values of an existing list.

There are three things needed for a python list to work.

- First is the expression we’d like to carry out. expression inside the square brackets.
- Second is the object that the expression will work on. item inside the square brackets.
- Finally, we need an iterable list of objects to build our new list from. list inside the square brackets.


## Creating a list with range

construct a basic list using range() and list comprehensions
syntax
[ expression for item in list ]
digits = [x for x in range(10)]

print(digits)

output: 

`[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]`