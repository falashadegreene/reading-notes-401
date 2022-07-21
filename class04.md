# Reading

## Classes and Objects

Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects. You can create multiple different objects that are of the same class. However, each object contains independent copies of the variables defined in the class. credit - https://www.learnpython.org/en/Classes_and_Objects

example of a class:

`class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")`

## Thinking Recursively

Thinking recursively essentially means to break down a problem to try and solve them in smaller chunks. According to the article If the current problem represents a simple case, solve it. If not, divide it into subproblems and apply the same strategy to them. A recursive function is a function defined in terms of itself via self-referential expressions. credit - https://realpython.com/python-thinking-recursively/  

A typical structure of a recursive algorithm in python below:

`houses = ["Eric's house", "Kenny's house", "Kyle's house", "Stan's house"]

def deliver_presents_recursively(houses):
    # Worker elf doing his work
    if len(houses) == 1:
        house = houses[0]
        print("Delivering presents to", house)

    # Manager elf doing his work
    else:
        mid = len(houses) // 2
        first_half = houses[:mid]
        second_half = houses[mid:]

        # Divides his work among two elves
        deliver_presents_recursively(first_half)
        deliver_presents_recursively(second_half)`

## Pytest Fixtures and Coverage

- Pytest fixtures are functions attached to the tests which run before the test function is executed.

- Coverage It monitors your program, that can note which parts of the code have been executed. 