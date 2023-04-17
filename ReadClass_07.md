# Read Topics: 07
## Variable Scope

A variable's scope defines the areas of the program where the variable can be used, and it's determined by where the variable is defined.

**Local Scope:** Variables defined within a function have a local scope, and they can only be accessed within that function. For example, if you define a name inside a function, it will only be accessed inside the function.

**Global scope:** Variables defined outside of a function or in the global space have global scope, and they can be accessed throughout the program. For example, if you define a variable above all functions, it will be accessible by all functions.

## Global vs. nonlocal

In Python, we can use the global and nonlocal keywords to access variables outside of the current scope. These keywords allow us to modify the value of variables defined in outer scopes.

## Big O importance

The Big O notation provides a way to quantify the relationship between the size of the input and the time required to solve the problem. This information is critical for developers and computer scientists because it helps them understand how the performance of an algorithm will change as the input size grows.

## Dice Roll Experiment

I simulated the dice rolling using the Random module, which provided the needed randomness in obtaining the expected outcomes of a dice.

To simulate the chance of getting a number (the probability of an outcome), First, I will need to define a counter that counts each time randint() gives me the wanted number (in this case 6), and then I will divide the counter by the number of trials or attempts.