# Pythonisms

## Dunder Methods

Dunder Methods are methods you can use to emulate behavior of built in types. So instead of `len('str')` a more effective method is to use a dunder `__len__` to add to class. 

1. Object Initialization - __init__ to create a constructor 
2. Object Representation - __str__, __repr__ provides a string representation of object
3. iteration - __len__, __getitem__, __reversed__  method to add transactions 


`class LenSupport:`
    `def __len__(self):`
        `return 42`

`>>> obj = LenSupport()`
`>>> len(obj)`
`42`

## Iterators

An iterator is an object that contains a countable number of values.

`class Repeater:`
    `def __init__(self, value):`
        `self.value = value`

    `def __iter__(self):`
        `return RepeaterIterator(self)`

## Generators

Python generators allows for you to create simplified iterators. Instead of using return statements it uses yield to pass data back to the caller.

`def repeater(value):`
    `while True:`
        `yield value`


## Things I want to know more about 

Interested in seeing more on dundar methods being used.
