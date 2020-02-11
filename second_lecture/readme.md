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
that come with it, such as `**addition**, **subtraction**, **multiplication**, **division**
and the **modulo** operator which returns the **remainder** of a division.`
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

> Possible exercises here:

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

> Possible exercise: Create two string variables of your choices and assign each a different username of your choice. Check what
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
