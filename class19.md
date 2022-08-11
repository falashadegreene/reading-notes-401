# Reading

## Python Regular Expressions Tutorial

1. import module `import re`

2. tackle basic patterns using ordinary characters:

 pattern = r"Cookie"
sequence = "Cookie"
if re.match(pattern, sequence):
    print("Match!")
else: print("Not a match!")
match!

3. a period matches any signle character except the newline character:

re.search(r'Co.k.e', 'Cookie').group()
'Cookie'

4. Repetitions checks if the preceding character appears one or more times starting from that postion.

5. Grouping in Regular expressions. It allows you to pick up parts of the matching text. 

## shutil

Shutil module in Python provides many functions of high-level operations on files and collections of files. It comes under Python's standard utility modules. This module helps in automating process of copying and removal of files and directorie
(credit: https://www.geeksforgeeks.org/python-shutil-which-method/#:~:text=Shutil%20module%20in%20Python%20provides,shutil.)

## copying files

shutil_copyfile.py
import glob
import shutil

print('BEFORE:', glob.glob('shutil_copyfile.*'))

shutil.copyfile('shutil_copyfile.py', 'shutil_copyfile.py.copy')

print('AFTER:', glob.glob('shutil_copyfile.*'))

## Things I want to know more about

Interested to see how shutil is utlized in automating of copying and removal of file directory.
