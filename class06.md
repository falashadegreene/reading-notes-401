# Reading

## How to use Random Module

According  to the random module provides access to functions that support many operations. Random module contains useful functions:

- randint function
- random
- choice
- Shuffle
- randrange

example code: 

`import random
import itertools

outcomes = { 'heads':0,
             'tails':0,
             }
sides = outcomes.keys()

for i in range(10000):
    outcomes[ random.choice(sides) ] += 1

print 'Heads:', outcomes['heads']
print 'Tails:', outcomes['tails']`


## What is Risk Analysis

Analysis risk the process of identifying the risks in applications or software that you built and prioritizing them to test. Using risk analysis at the beginning of a project highlights the potential problem areas. (credit: https://www.edureka.co/blog/risk-analysis-in-software-testing/ )

possible risk encounters: 

- Use of new hardware
- Use of new technology
- Use of new automation tool
- The sequence of code
- Availability of test resources for the application.

## Test Coverage

Test coverage is a used for finding untested parts of a codebase. It monitors your program, noting which parts of the code have been executed.  