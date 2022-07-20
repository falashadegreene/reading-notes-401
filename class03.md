# Reading

## Reading and writing files in Python

A file is a contiguous set of bytes used to store data. File systems are made up of Header, Data and End file. See below:

- Header: metadata about the contents of the file (file name, size, type, and so on)
- Data: contents of the file as written by the creator or editor
- End of file (EOF): special character that indicates the end of the file 

## Opening and closing a file in Python

To open a file you will have to invoke it with the open() built in function. Example `file = open('dog_breeds.txt')`. After opening a file you want to make sure you  close it. closing your file is important because it is best practice and it can prevent unwanted behavior. To  properly close a file you can use a try-finally block. Below example: 

`reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()`

## Exceptions in Python

Syntax Errors are  when  the parser detects a incorrect  statement. According to the article a exception error occurs whenever syntactically correct Python code results in an error. The last line of the message indicated what type of exception error you ran into.

## Things I want to know more about

I would like to learn more about raising an exception and assertation errors. Is this method another way to bypass the error? Not too clear on the explantion in the article. 