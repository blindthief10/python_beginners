# third lecture

## Previous lecture revision

**What did we cover last week?**

1. String functions and slicing strings
2. Boolean values
3. Comparison operators
4. Logical operators
5. Create random numbers with random module
6. Conditional statements
7. While and for loops

### Casting

1. str() function to convert to string
2. int() function to convert to integer
3. float() function to convert to float etc.

#### Recap exercises

1. Iterating through strings with for loop, using the range function, or directly.

> Find if a positive integer is a special number or not.
* Special number is considered the number whose digits consist of **0**, **1**, **2**, **3**, **4**, **5**
* Examples of special numbers are: **14**, **22**, **35** etc.
* Non-special numbers are: **9**, **17**, **63** etc.
* [Feel free to find the original exercise here](https://www.codewars.com/kata/5a55f04be6be383a50000187)

>Find if a positive integer is a jumping number or not.
* Jumping number is the number whose all consecutive digits have difference 1 with one another.
* Such example would be: **123**, **4543**, **2345434**, etc.
* All single-digit numbers are considered as jumping numbers.
** [Feel free to find the original exercise here](https://www.codewars.com/kata/5a54e796b3bfa8932c0000ed)

#### Working with lists

1. What are lists meant for? A collection of data types regarding a specific thing. All heights, all scores, all names etc
2. Select elements by index, slice arrays.
3. Functions work like string functions with one exception. They happen in place
4. Some useful functions you will need:
  * `len()`. Indicates how many elements the list contains
  * `append()` Insert a new element at the end of the list
  * `insert()` insert's an element at the given index
  * `remove()` removes the element with the given value
  * `pop()` removes the element at the given index. If no index is passed, then the last element is removed
  * `count()` counts how many times an element is found within the list
5. The `in` operator that returns a boolean. Checks if an element is in the list or not
6. Iterate through all list's elements is possible
> Lists play a vital role to python, as a programming language and in data science field in particular. So feel
free to [learn more about lists here](https://www.w3schools.com/python/python_lists.asp)

#### Advanced List comprehension

> How to create lists in a very compact way. Syntax

#### Lists exercises

> Rolling a die histogram
* Create an empty list. Populate this list with 50 random integers between 1 and 6. After that display your results like a
histogram as it's shown [here](https://www.codewars.com/kata/57d532d2164a67cded0001c7).

> Create 2 empty lists. These lists should hold all test scores of participants for a given test in 2 different classes.
* The range of participants is unknown but it should be between 50 and 100 randomly.
* Each test score should be an random integer between 0 and 100.
* Find out first which class has more participants.
* Find out which class has a bigger average score than the other. Using the `sum()` function could be helpful here, since
you can already calculate the number of items within the list.
* **Bonus challenge**: Calculate also the variance for each list. variance is the sum of squares of differences between each value and the average, divided by the length of the sample - 1. For example ((x1-avg) ** 2 + (x2-avg) ** 2 + ... + (xn - avg) ** 2 ) / sample's length - 1).
* **Bonus nr2** Calculate the standard deviation for each list. Standard deviation is the simply variance's square root.
* **Extra Bonus**: What is the percentage of students who failed the test. Whose score was below 50 in other words.

> Santa Klaus naughty list. Help Santa to detect and filter who deserves to have gifts or not.
* Candidates are: Anna, Bill, James, Jake, Jessica, John, Niels, Marco, Chris, Laura, Bettina, George
* The naughty list is comprised of: Chris, Jessica and Bill
Write a piece of code that prints to the console the names of those who deserve to take a gift from Santa.

#### Working with dictionaries

1. Dictionaries. Differences with lists. Named indexes. Multiple data types, different purposes.
2. Keys and values of dictionaries. Accessing a specific value by key.
3. Removing a key from a dictionary, adding a key-value pair to a dictionary,
4. Set default values for a new key-value pair

#### Dictionaries' exercises

> First Exercise example: Users and premium accounts together

> You work as a salesman in a small shop that sells electronic devices. Mainly laptops, desktops, mobiles, headphones
and cables. For each sell you just append the type of the item at the end of a list which contains all sold items for
the day.
At the end of the day your list is the followed:

> ['headphones','desktop','headphones','mobile','mobile','desktop','laptop','headphones','desktop','desktop','cable']
> Write a piece of code that makes of use of this data to summarize a dictionary that depicts how many items were sold by category.
For example: {'headphones': 3, 'mobile': 2, 'laptop': 1, 'cable': 1, 'desktop': 4}

#### Write reusable code with functions

> How do we define a function with `def my_function()` keyword definition
> Execute the dictionary sales transformation function above at will by encapsulating it in a function
> Re use this with any kind of data by using arguments
> The  `return` keyword and it's use

##### Further exercises with function

* Write a function that accepts a list of strings as an argument and returns it's biggest string
* Write a function that accepts Fahrenheit degrees and converts it into Celsius degrees for temperature [Find the formula here](https://www.rapidtables.com/convert/temperature/fahrenheit-to-celsius.html)
* Write a function that given a list of tests, returns the length of participants, their average score,
the variance, the standard deviation and the failure percentage in a dictionary with meaningful keys.
