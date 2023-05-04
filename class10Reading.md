# List Comprehensions in Python
In order to explain exactly what is list comprehension I will answer three questions:What, Why, How.

## What is list comprhension 
List comprehension is a powerful and concise method in python for creating lists.
<b>Syntax</b>
  new_list= [ expression for item in list ]

at this syntaxis three main parts:
1- the expression that will perform on each item. 
2- the object that the expression will implement on; in this case the item. 
3- the iterable list of the objects that will iterate on.

## Why using list comprehension 
we use the list comprhension because it is more managable, compact, elegant and readable way than the for loop.

example:
<pre>
nums = [x+y for x in [1,2,3] for y in [10,20,30]]
print(nums)

output: [11, 21, 31, 12, 22, 32, 13, 23, 33]
</pre>

as you notice in this example if you use the normal for loop you will a nested for loop and it will look like that:
<pre>
result = []
for x in [1, 2, 3]:
    for y in [10, 20, 30]:
        result.append(x + y)
        </pre>
 I hope it is obvious for you now why we use comprhension we work with lists in python.

## How to use list comprehensions
In this part I will talk about using comprehensions with diffrent type of expressions and some extras to syntax.

##### we can at first simply use in creating a simple list from range of number like this:
<pre>
digits = [x for x in range(10)]

print(digits)

#output
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
</pre>

##### or we can use it to create another list with a simple expression like this:
<pre>
multiples_of_three = [ x*3 for x in range(10) ]

print(multiples_of_three)

#output
[0, 3, 6, 9, 12, 15, 18, 21, 24, 27]
</pre>

##### and we can use filter with to have a list that match our condition:
<pre>
even_numbers = [ x for x in range(1,20) if x % 2 == 0]
print(even_numbers)

#output
[2, 4, 6, 8, 10, 12, 14, 16, 18]
</pre>

##### also the expression can simply a funtion:
<pre>
lower_case = [ letter.lower() for letter in ['A','B','C'] ]
print(lower_case)

#output
['a', 'b', 'c']
</pre>

##### we also can use to extract digits from a string contains letters and digits:
<pre>
user_data = "Elvis Presley 987-654-3210"
phone_number = [ x for x in user_data if x.isdigit()]

print(phone_number)

#output
['9', '8', '7', '6', '5', '4', '3', '2', '1', '0']
</pre>

##### we can use string methods with it:
<pre>
authors = ["Ernest Hemingway","Langston Hughes","Frank Herbert","Toni Morrison",
    "Emily Dickson","Stephen King"]

# create an acronym from the first letter of the author's names
letters = [ name[0] for name in authors ]
print(letters)

#output:
['E', 'L', 'F', 'T', 'E', 'S']
</pre>

And a lot of other uses.

### In conclusion
List comprehensions have great potential in writing more elegant Python code. It is important to write compact code when working with teams and maintaining programs. 
By learning advanced features like list comprehension, you can save time and enhance productivity. Your colleagues will appreciate your code that is more concise and 
easy to read, and you will thank yourself when you revisit a program after months and find the code manageable.

