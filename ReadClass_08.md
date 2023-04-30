# Read Topics: 08

## List Comprehension

The basic syntac of Python list comrhension is as follows:
list_name=[The expression you desire.]

List comprehension differs from using a for loop to create a list in terms of syntax and readability. List comprehension allows you to write the creation of a new list in a single line of code, making it more concise and readable. 

list = [1, 2, 3, 4, 5]
squared_list = [x*2 for x in list]
print(squared_list)


## Python Decorator

from it's name a decorator is a design pattern that allows you to modify the behavior of a function or class without changing its source code directly.
 
A decorator is a Python object that takes another function or class as input, and returns a new function or class that adds some extra functionality to the original one.

*Concept:* 

Decorators in Python are functions that modify the behavior of other functions or classes without changing their source code.

*Use cases:* 

1- Logging: Adding logging functionality to a function or class to track its usage and behavior.

2- Timing: Measuring the time taken to execute a function.

3- Caching: Storing the results of a function in memory to avoid recomputing them on subsequent calls.

Example: 
```
def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

def say_whee():
    print("Whee!")

say_whee = my_decorator(say_whee)
```
With an output of :

```
>>> say_whee()
Something is happening before the function is called.
Whee!
Something is happening after the function is called.
```