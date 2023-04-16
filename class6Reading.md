# Class 06 Readings

## Utlizing random module in python to create random or make selections from a list
 The Random module contains some very useful functions namely randint() function, random() function, choice() function, randrange() function and shuffle() function.

### Common functions available in random module
   
#### Radiant() : The randint() function can be used to create random strings within a range. The function takes two numbers as its input argument. The first input argument is the start of the range and the second input argument is the end of the range. returns a random integer within the given range.

#### Random() : the random() method is used to generate random numbers between 0 and 1. When executed, the random() function returns a floating point number between 0 and 1.

#### Choise() : The choice() function is used to select a random element from a collection object like a list, set, tuple, etc. The function takes a collection object as its input argument and returns a random element.

#### Shuffle() : the shuffle function shuffles the elements in the list in place. The shuffle() function takes a list as an input argument. After execution, the elements of the list are shuffled in a random order as shown in the following example.

#### Randrange() : the randrange() is used to select a random element from a given range. It takes three numbers namely start, stop, and step as input argument. After execution, it generates a randomly selected element from the range(start, stop, step). To understand the working of range() function
   
## Risk Analysis
  Risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done. The categorization of the risks takes place, hence, the impact of the risk is calculated.
   
### The key steps involved in conducting a risk analysis for a software project   
   * Conduct Risk Assessment review meeting

   * Use maximum resources to work on high-risk areas

   * Create a Risk Assessment database for future use

   * Identify and notice the risk magnitude indicators: high, medium, low.
     
## Test Coverage
     Test coverage is a useful tool for finding untested parts of a codebase. Test coverage is of little use as a numeric statement of how good your tests are.
       
### The importance of test coverage
      it helps you find which bits of your code aren't being tested. People focus on coverage numbers is because they want to know if they are testing enough.
### How it can be missleading
       The trouble is that high coverage numbers are too easy to reach with low quality testing. At the most absurd level you have AssertionFreeTesting. But even without that you get lots of tests looking for things that rarely go wrong distracting you from testing the things that really matter.
 
## Big O Notation
    Is how time scaled with respect of some input variables .     

### describe the performance of an algorathim 
 * diffrent steps get added :An algorithm consists of a series of steps that it follows to solve a problem. The time it takes to perform each step can vary, and the total time required to solve the problem is the sum of the time required for each step.
 * drop constants :  In analyzing the performance of an algorithm, we typically ignore constant factors that do not depend on the input size. This is because these factors do not affect the overall growth rate of the algorithm's running time as the input size increases. For example, if an algorithm takes 3n + 2 steps to solve a problem, we would simplify this to O(n), because the constant factors (3 and 2) are dropped.
 * diffrent inputs == diffrent variabls : The performance of an algorithm can vary depending on the input size. For example, sorting an array of 100 elements will typically take longer than sorting an array of 10 elements. We use different variables to represent different input sizes in order to analyze how the algorithm's performance scales as the input size increases.
 * Drop non-dominate terms : When analyzing the time complexity of an algorithm, we typically focus on the dominant term (i.e., the term with the largest exponent) and drop any non-dominant terms. This is because as the input size increases, the contribution of the dominant term to the running time of the algorithm will become increasingly significant, while the contribution of the non-dominant terms will become relatively smaller. For example, if an algorithm has a time complexity of O(n^2 + n), we would simplify this to O(n^2), because the n^2 term dominates the n term as n gets larger

### An example of an everyday task that demonstrates O(n) time complexity          
Is counting the number of items in a grocery bag. Assuming you have a grocery bag with n items, you can count the items by simply scanning each item in the bag one by one until you reach the end of the bag. This means that the time it takes to count the items increases linearly with the number of items in the bag. In other words, the time complexity of this task is O(n), where n is the number of items in the bag.

If you double the number of items in the bag, the time it takes to count them will also double. Similarly, if you halve the number of items, the time it takes to count them will also be halved. This linear relationship between the input size (number of items) and the time required to perform the task is what characterizes O(n) time complexity.
