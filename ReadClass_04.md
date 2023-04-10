# Reading Topic


I found this topic extremely useful as it defined the difference between the concepts of Objects and Classes also, Introduced me to fixtures.


## Classes & Objects
Classes is essentially is a template that contains the attributes and functions.
While the Object is an instance from the class with it's own set values from that class.


How we use them:


1- Create a class with methods (functions) and attributes.
2- Create an instance (Object) from that class.
3- Modify the attributes of that instances.


## Thinking Recursively


Recursion is a programming technique in which a function calls itself to solve a problem, an obvious example of recursion is to calculate the factorial of a number.


def factorial(num):
    if num == 0:
        return 1
    else:
        return num * factorial(num-1)


**Best Practices:**


1- Define a base case.
2- Test the function.
3- Decompose the original problem into simpler instances
4- insure that you won't get stuck in an infinite loop.



## Pytest Fixtures


In testing our code, a fixture provides a defined, reliable and consistent context for the tests.


By using pytest fixtures and code coverage together, you can improve the quality and maintainability of your project in several ways:


1- Consistency: fixtures ensure that the same setup code is executed before each test
2- Reusability: fixtures can be reused across multiple tests.
3- Maintainability: By ensuring that your tests cover a high percentage of your code, you can make it easier to maintain and update.