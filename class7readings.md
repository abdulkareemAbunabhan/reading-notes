# Class 07 Readings

## the concept of variable scope in Python and describe the difference between local and global scope. 
 In Python, variable scope refers to the part of the program where a variable is accessible. A variable's scope determines where in the code that variable can be accessed and modified.

There are two types of variable scopes in Python: local scope and global scope.

* Local Scope: Variables defined inside a function have a local scope, which means that they can only be accessed within that function. When a function is called, the variables inside it are created, and when the function completes, they are destroyed. Attempting to access a local variable outside of its function will result in a NameError.
Example:

<pre>
```python
def my_function():
    x = 10
    print(x)

my_function() # Output: 10
print(x) # Error: NameError: name 'x' is not defined
```
</pre>

* Global Scope: Variables defined outside of any function or class have a global scope, which means that they can be accessed from anywhere in the code. Global variables can be accessed and modified by any function or class that has access to the global namespace. However, it is generally recommended to avoid using global variables because they can cause naming conflicts and make it difficult to debug code.
Example:
<pre>
'''python
x = 10

def my_function():
    print(x)

my_function() # Output: 10
print(x) # Output: 10
'''
</pre>

## global and nonlocal are keywords

global is used to refer to a variable in the global scope, i.e., a variable declared outside any function. When we use the global keyword, we can access the variable in the function and also modify its value. For example:

<pre>
```python
x = 10

def my_function():
    global x
    x = 5
    print(x)
    
my_function()  # Output: 5
print(x)       # Output: 5
```
</pre>

Here, we used the global keyword to access the global variable x and modified its value inside the function.

nonlocal is used to refer to a variable in the outer (enclosing) local scope of a nested function. In other words, when we have a nested function, the nonlocal keyword allows us to access the variable in the outer function and modify its value. For example:

<pre>
```python
def outer_function():
    x = "local"
    def inner_function():
        nonlocal x
        x = "nonlocal"
        print("inner function: ", x)
    inner_function()
    print("outer function: ", x)

outer_function()  # Output: inner function: nonlocal, outer function: nonlocal
```
</pre>

## Big O purpose and importance
The purpose of Big O notation is to analyze and describe the time and space complexity of algorithms. It helps to evaluate the efficiency of different algorithms and to choose the most appropriate one for a given problem. By using Big O notation, we can quantify the performance of an algorithm in terms of how the running time or memory usage scales with the size of the input. This information is essential for developing efficient and scalable software solutions. In summary, Big O notation is a vital tool for algorithm analysis, optimization, and comparison.
and the importance of it that it heps us use the right data structure and the right algorithm depending on our code and problem.

## simulate a dice roll

To simulate a dice roll using Python, we can use the random module which provides a randint function to generate random integers between a given range. Since a dice has six sides, we can use the randint function to generate a random number between 1 and 6, inclusive, to simulate a dice roll.

Here's an example code snippet to simulate a dice roll using Python:
<pre>
```python
import random

# Simulate a dice roll
dice_roll = random.randint(1, 6)
print("The dice rolled:", dice_roll)
```
</pre>

To calculate the probability of rolling a specific number over a large number of trials, we can use a loop to simulate multiple dice rolls and count the number of times the specific number is rolled. We can then divide the count by the total number of trials to get the probability.

Here's an example code snippet to calculate the probability of rolling a 6 over 10,000 trials:

<pre>
```python
import random

# Set the number of trials
num_trials = 10000

# Initialize the count
count = 0

# Simulate the dice rolls
for i in range(num_trials):
    dice_roll = random.randint(1, 6)
    if dice_roll == 6:
        count += 1

# Calculate the probability
probability = count / num_trials

# Print the result
print("The probability of rolling a 6 in", num_trials, "trials is:", probability)
```
</pre>
This code snippet uses a loop to simulate 10,000 dice rolls and counts the number of times a 6 is rolled. It then divides the count by the total number of trials to get the probability of rolling a 6. The output might look something like this:

<pre>
```python
The probability of rolling a 6 in 10000 trials is: 0.1695
```
</pre>
This means that over 10,000 trials, the probability of rolling a 6 is approximately 16.95%.
