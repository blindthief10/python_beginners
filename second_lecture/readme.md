# Second Lecture

## Previous lecture revision

**What did we cover last week?**

1. What is Python and on what kind of applications can be used to?
2. Choosing our text editor or IDE to write our first python code.
3. The `print` function to print something directly to the console.
4. We learned about different `data types`. What do they mean and why should we care.
5. We saw how to detect the type of a value by using the `type` function.
6. We wrote `comments` to document our code. Both single-line and multi-line.
7. An introduction to `int` (**integer**) data type and all basic math operations
that come with it, such as **addition**, **subtraction**, **multiplication**, **division**
and the **modulo** operator which returns the **remainder** of a division.
8. We imported the `math` module and used `sqrt` function to calculate the square root of a number.
9. We created our first `strings`. Used the `+` operator, in order to concatenate multiple strings
into one.
10. We used the `format` string function in order to inject multiple values inside our string.
11. We learned how to create variables, store values there, update the values of these variables and
reference them by name later. We talked about **snake_case** ex:(`first_name = 'Jake'`) and **camelCase**
ex: (`firstName = 'Jake'`) convention naming.

## Second lecture's content

#### A closer look to strings and other functions

> **Strings are immutable** data types. That means that whenever we are trying to apply
a function on a current string, the transformation does not effect the initial string, rather it
returns a new temporary string

Some examples follow, in order to make this concept as clear as possible

**Notable string functions** and examples

> `first_name = 'Jake'
print(first_name.upper()) #prints 'JAKE' to the console
`

> `print(first_name.lower()) #print 'jake' to the console`

> `print(len(first_name)) #prints how many characters and empty spaces the string is comprised of. It's an integer`

**Notable tip**: Try to print again the variable itself after all these actions. What do you see? Is it what you expected?

[Feel free to find all string attached functions here](https://www.w3schools.com/python/python_strings.asp)

#### Selecting specific letters or slicing strings by indexing. How does **index** work?

> Explain the starting index **(inclusive)**, end index **(not inclusive)**, and step

1. Select the first letter of a name
2. Select the last letter of a name
3. Select everything except the first two letters
4. Select the last three letters
5. Select and print the reversed version of the name

#### Boolean values

What are **boolean** values and how many possible values can they take? What do these values represent? True, False, Both?

> Create a variable and assign a boolean value to it, the variable should correspond to whether it's raining right now or not.
Print the variable and it's type in order to get familiar with the new data type.

How can we create boolean values?

1. By directly assigning `truthy` or `falsy` values.
2. By comparing. That means by using `comparison operators` for checking equality, inequality, greater than, lower than etc.

> Such symbols are:
1. `==` equality checking
2. `>` greater than
3. `<` lower than
4. `>=` greater than or equal
5. `<=` less than or equal
6. `!=` not equal, checking inequality

These **comparison operators** can be combined with **arithmetical operators** we learned during previous lectures.
In such case, arithmetical operators **always execute first**, comparison operators follow after.

> If you want to learn more about the order of precedence [check this out](https://www.programiz.com/python-programming/precedence-associativity)

> An example would be checking the following code `5 + 2 > 10 - 4`. This expression should evaluate to True as 7 is greater
than 6

> Coding challenge: Create two string variables of your choices and assign each a different username of your choice. Check what
is the outcome of comparison by assuming that the first string is longer than the second one. Remove any unused space before and after each string, before making the comparison.

3. Combining such statements with **logical operators**

> Mainly python offers three logical operators for calculating the outcome of multiple boolean values:
1. **and** both sides have to be true, in order for the whole expression to evaluate to true
2. **or** at least one side should be true, in order for the whole expression to evaluate to true
3. **not** which evaluates the expression of the boolean to it's opposite.
**Please Notice**: Logical operators still execute in a specific order that is described above.

> Create 3 variables, named **is_sunny**, **is_raining**, **is_snowing**. Feel free to assign boolean values of your choice.
I would like to make three questions based on these facts. Use the correct logical operators to answer and print outcome.
1. Is there any chance observing a rainbow?
2. Is the weather generally bad? Does it rain or snow?
3. I would like to go out, but only if it doesn't snow. Should I go?

> Create a variable and assign a random integer into it. The integer should represent a given year (like 2019 etc).
Print to the console if the given year is a bisect or not. Knowing that we have a bisect year every 4 years (2000, 2004, 2008)
should help.
**Bonus challenge**: We also know that 2000 was bisect, but 1900, 2100, 2200, 2300 will be not. In fact, during the change of century the years are not bisects. There is an exception to the rule though that occurs every 400 years. Thus 1600 AD, 2000 AD, 2400 AD were and will be bisect years. Add a complexity to your existing code to additionally predict this fact.


#### Import the random module to create random numbers

> Use the `random` function of the `random` module to create a random number between 0 and 1. Print, in the form of boolean if the random number you just
generated is bigger than 0.5 or not. (print also the number if you like).

> Use the `randint` function of the `random` module to create a random integer between a range (let's say from 1 to 5) (both ends inclusive). And another variable which is a number of your choice. Check if you have guessed the number that was created randomly.

#### Conditional flow with if statements

1. `If` statement syntax (indentation) explained. How to spot which block of code will be executed and when.

> Print a meaningful message to the console if you have guessed correctly the number from above challenge.

2. `Else` statement. When this block will be executed? Used as a default block

> Print a meaningful message to the console if the random number is different than the one you guessed.

> Create a random integer from 1 to 100 and check if it's an odd number or even number.

3. `elif` statements. Checking multiple times for more than one additional conditions.

> Create 2 random integers from 1 to 10. Check if number A is bigger, if number B is bigger or if they are equal.

> Re-write the leap year problem with if... else conditional blocks.
**Bonus challenge** Do not use any logical operators (and, or, not) inside your if conditions. For any case print a
relevant message to the console depending on, if the checked year is a leap year or not.

> **The fizz_buzz problem**
Create a number of your choice from 1 to 100.
1. If the number is a multiple of 3 print to the console 'Fizz'
2. If the number is multiple of 5 print to the console 'Buzz'
3. If the number is both multiple of 3 and 5, print 'FizzBuzz'
4. In any other case print the number itself.

> **Check palindrome problem**
Create a variable and assign a name of your choice to it.
* Check if the name you assigned is a palindrome or not. Palindrome means, that the name can be written exactly the same
if you reverse it.
* Ignore case sensitivity and strip it before checking.
* Print a descriptive message to inform the user if the name is a palindrome or not. (A good example is 'Anna').

> Lottery winnings calculator
* Create a random integer from 1 up to 100. This is the winning number for this lottery.
* Create a second variable which is your guessing integer.
* If you guessed correctly then the prize is 100$.
* If the number you guessed is less than or equal to 10 numbers away from the winning number then you win the 100$
but you lose 10$ for every number you are apart. For example, if the winning number is 68 and you have guessed 64. Then you win 60$, if you guessed 77 then you win 10$ etc.
* In any other case you win nothing.
* For all cases print both numbers, and the winnings that were calculated.

#### Repeat code execution with loops

1. The while loop lifecycle example
2. Syntax indentation
3. Avoid infinite loops with correct condition, updating the value inside the loop and with the usage of the `break` keyword
4. Different kinds of loops. `while` vs `for`. Use cases. Known vs unknown trials.

> Print all numbers from 1 to 100

> Print all even numbers from 1 to 100. Ignore the odd numbers.

> Refactor the FizzBuzz problem so that it does the same thing for all numbers from 1 to 100 and not only for one number.

> Imagine that you work at sales department in a clothing-shop and you are responsible for selling 3 products:
A t-shirt that costs 10$. A pair of Jeans that costs 30$, and a Jacket that costs 150$
You have noticed a paradox pattern. Every three customers, each new customer buys the same things.
For example the first customer buys 3 t-shirts. The second customer buys a 2 Jeans. The third customer buys a jacket.
And then again the same from the beginning.
The fourth customer again 3 t-shirts. The fifth customer buys again 2 jeans. The sixth customer buys again one jacket.
That continues until the end of the day.
Find out how much money your cashier has if the initial cashier was already at 150$ and the total number of customers at the end of the day was 78.

> Solve the ship container problem
* Suppose you own a ship. This is ship can carry up to 10.000 Kg in terms of weight.
* A merchant wants you to carry his goods with your ship.
* He has 500 containers and he wants you to carry as many as possible. All containers have an identifying number from 1 to 500.
* The first 100 containers weight 10Kg each.
* The containers with number from 101 up to 200 (included) weight 20kg each.
* The containers with number from 201 up to 250 (included) weight 50kg each.
* The containers with number from 251 up to 300 (included) weight 100kg each.
* The containers with number from 301 up to 400 (included) weight 200kg each.
* The rest weight 500 Kg each.
* Put as many containers as possible without sinking your ship. Find a way to stop adding weight if you surpass the limit your ship can afford.
* Print to the console exact how many containers you have included to your ship and how much is the difference between the total weight of the containers and the weight your ship can afford (free available weight).
