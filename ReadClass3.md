# FileIO & Exceptions

## What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?

In Python, the with statement is used when working with files to ensure that the file is properly closed after the block of code is executed.

## Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method?

In Python, the read() and readline() methods are used to read data from a file object. The main difference between these two methods is that read() reads the entire contents of the file into a string, whereas readline() reads one line of the file at a time.

for example:

with open('file.txt', 'r') as file:

    contents = file.read()
    line1 = file.readline()
    print(contents)

here, contents will equal the entire string file, whereas Line1 will equal that exact line only.

## Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.

Exception handling is a concept in Python that allows you to handle errors and exceptions that may occur during the execution of a program. When an error or exception occurs, it can be caught and handled in a way that allows the program to continue running without crashing.

for example:

try: 

x=1/0

except Divide_On_zero:

print("error you divided on zero man!")

finally:

print("Done")