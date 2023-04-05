# Reading topics:

These topics are crucial to our path of coding, as they will greatly help us to follow a methodology of writing code to ensure that it works efficiently and is bug-free.

Also, it introduces us to some new concepts and previous ones and explains the differences between modules and packages.

## In Tests We Trust: TDD with Python

Based on what I've learned, the lean principle of TDD is to think about the test first, and then and only then write the tests that will provide both the input and the output.

The contribution of the TDD method enhances the overall quality of the written code since you catch bugs early on and fix them immediately (be your own QA!).

## If name == main

The Python interpreter reads the source file and defines a few special variables and global variables. For its use cases: If the Python interpreter is running that module (the source file) as the main program, it sets the special name variable to have a value of "main". If this file is being imported from another module, the name will be set to the module’s name.

So, to sum it up, it is used to check whether the current file is being executed as the main program or whether it is being imported as a module into another program.

## Recursion in Python

Recursion is a concept used in most of the programming languages, as it's a function that keeps calling itself repeatedly until it reaches its specified target (Base Case).

Recursion is a great tool if used correctly, as if you misuse it, you may run into an infinite loop hole, or a black hole, if I dare say that.

## Differences between Python modules and packages

Modules are single files containing Python code, while packages are directories that can contain one or more modules or sub-packages.

To create a module in Python, you simply create a file that has an extension of ".py" and then insert all the functions, variables, and classes that you want in it.

On the other hand, to create a package, you need to create a directory with an "init.py" file inside. You can then add one or more module files to the package directory.

To import a module, you simply follow this: Import Module_Name, while to import a package, you should install the package, then from Package_Name, import Wanted_Module.

## Things I want to know more about

None currently.