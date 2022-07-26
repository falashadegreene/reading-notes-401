# Reading

## Python Scope

## Global

Assigning a value to a name outside of all functions at maybe the top level of a module then it is considered a global python scope.

## nonlocal

Assigning a value to a name inside a function. That name will have a local python scope.

**Enclosing** - (or nonlocal) scope is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. This scope contains the names that you define in the enclosing function. The names in the enclosing scope are visible from the code of the inner and enclosing functions. (credit: https://realpython.com/python-scope-legb-rule/ )


**Global** (or module) scope is the top-most scope in a Python program, script, or module. This Python scope contains all of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.  (credit: https://realpython.com/python-scope-legb-rule/ )


