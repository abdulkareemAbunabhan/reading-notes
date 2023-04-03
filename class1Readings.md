#### the main challenges faced by beginners when learning Python
* having to think your way through problems that you had only even heard about a few hours beforehand.
* research for hours on end, fleshing out the skeleton that we discuss in class, piling information on top of application so that you can reach your goals.
* constantly confronted with your own lack of understanding of a topic.
* they will have to forge your own path toward a solution.

#### strategies for overcoming these obstacles.
1. Practice regularly: Practice is key to mastering any skill, including programming. Try to code for at least an hour every day to build up your skills gradually.
2. Break down problems into smaller pieces: When you encounter a challenging problem, break it down into smaller pieces that you can tackle one by one. This approach can make the problem more manageable and less daunting.
3. Collaborate with others: Learning with others can help you stay motivated and gain different perspectives on problems. Look for online communities or meetups in your area to connect with other Python learners.
4. Stay organized: Keep your notes, code, and resources organized so that you can easily find what you need when you need it. This can save you time and reduce frustration.

### Big O notation:

* Time complexity refers to the amount of time an algorithm takes to complete its execution, given a particular input size. It is often expressed in terms of the "order of growth" of the algorithm, denoted by Big O notation. For example, an algorithm with a time complexity of O(n) means that the time it takes to complete will increase linearly with the size of the input. An algorithm with a time complexity of O(n^2) means that the time it takes to complete will increase exponentially with the size of the input.
* Space complexity refers to the amount of memory an algorithm needs to complete its execution, given a particular input size. It is also often expressed in terms of the "order of growth" of the algorithm, denoted by Big O notation. For example, an algorithm with a space complexity of O(n) means that the amount of memory it requires will increase linearly with the size of the input. An algorithm with a space complexity of O(n^2) means that the amount of memory it requires will increase exponentially with the size of the input.
* Both time complexity and space complexity are important considerations when designing and analyzing algorithms, especially for large or complex input sizes. By understanding these concepts, programmers can make informed decisions about the trade-offs between performance and memory usage, and choose the best algorithm for a particular problem.

### the difference between mutable and immutable data types in Python.

In Python, mutable and immutable are two basic categories of data types. The main difference between them is that mutable objects can be changed after they are created, while immutable objects cannot be changed once they are created.

Mutable objects are objects whose value can be modified after they are created. When an object is mutable, it means that you can change its value without creating a new object. Examples of mutable objects in Python include lists, dictionaries, and sets. For instance, if you have a list in Python, you can change its elements or append new ones without creating a new list. Here's an example:

<pre>
```python
>>> a = [1, 2, 3]
>>> a[1] = 4
>>> print(a)
[1, 4, 3]
```
</pre>

On the other hand, immutable objects are objects whose value cannot be changed after they are created. When an object is immutable, it means that you cannot modify its value. Examples of immutable objects in Python include strings, tuples, and numbers. Once an immutable object is created, you cannot change its value. Here's an example:

<pre>
```python
>>> a = "hello"
>>> a[1] = "E"  # This will raise an error since strings are immutable in Python
TypeError: 'str' object does not support item assignment
```
</pre>

It is important to note that when you modify a mutable object in Python, you are actually changing the object in place, which means that all variables that reference that object will reflect the changes. However, when you modify an immutable object, Python creates a new object with the new value and reassigns the variable to reference the new object, which can be inefficient in terms of memory usage.

In summary, mutable objects can be changed after they are created, while immutable objects cannot be changed once they are created. Understanding the difference between mutable and immutable objects is crucial in Python programming, as it can help you write more efficient and bug-free code.

## __Things I want to know more about__
