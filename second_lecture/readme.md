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

1. Select the first letter of a name
2. Select the last letter of a name
3. Select everything except the first two letters
4. Select the last three letters
5. Select and print the reversed version of the name
