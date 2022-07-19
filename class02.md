# Reading

## In Tests We Trust - TDD with Python

According to the blog Unit tests are pieces of code to exercise the input, the output and the behaviour of your code. When writing out test documentation it will need to be structured by Arrange, Act and Assert, then execute the test. Example of unit test below:

`def test_should_return_female_when_the_name_is_from_female_gender():
    detector = GenderDetector()
    expected_gender = detector.run(‘Ana’)
    assert expected_gender == ‘female’`

## If name equals main

In the GeeksforGeeks article it reads that before executing code, Python interpreter reads source file and define few special variables/global variables.
If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable.

A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended.(credit, GeeksforGeeks article)

## Recursion

Recursion is the process in which a function calls itself directly or indirectly and the corresponding function is called a recursive function. Recursion is a helpful technique in which it can reduce the length of code and make it easier to read and write. Properties of recursion are:

- Performing the same operations multiple times   with different inputs.
- In every step, we try smaller inputs to make the problem smaller.
- Base condition is needed to stop the recursion otherwise infinite loop will occur.
