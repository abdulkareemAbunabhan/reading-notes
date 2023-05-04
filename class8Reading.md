# The basic syntax of Python list comprehension
List comprehension is a powerful and concise method in python for creating lists.
<b>Syntax</b>
new_list= [ expression for item in list ]

at this syntaxis three main parts:
1- the expression that will perform on each item.
2- the object that the expression will implement on; in this case the item.
3- the iterable list of the objects that will iterate on.

### The difference from using a for loop to create a list
To understand the diffrence between using comprehension and a normal for loop to create a list in Python we will the same list in the both ways in example.
we will create a list for the first 10 numbers raised by the power of 2:

1- using for loop:
#create a list using a for loop
squares = []

for x in range(10):
    #raise x to the power of 2
    squares.append(x**2)
2- using comprehension
#create a list using list comprehension
squares = [x**2 for x in range(10)]

these two ways gives the same output but it is clear even on a simple example that the compprhension way reduce code and it is more elegant and compact.

In conclusion the comprhension method makes the code more readable,more managable, elegant, easy to understand and compact.

## Decorator in Python
Decorator is a function that takes another function and extends the behavior of the latter function without explicitly modifying it.
Example:
<pre>
```python
def my_decorator(func):
    def wrapper():
        print("Something is happening before the function is called.")
        func()
        print("Something is happening after the function is called.")
    return wrapper

def say_whee():
    print("Whee!")

say_whee = my_decorator(say_whee)```
</pre>

what happens here that the decartor funtion that takes a function as an argument adds some modifiying to the argument function in an inner function called wrapper and 
calling the argument funtion in the wrapper and returns the wrapper function without calling it, then we set the decorator that takes this function as an argument to a 
variable then we can called when ever we want by using the var name with parantecies.


### The concept of decorators in Python

the concept of the decorator is add some context or small modifying to behavior of a function without explicitly modifying the main function.

## Things I want to know more about
