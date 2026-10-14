# How Does the Print Function Work?

## 1. What Is the Terminal?

The **terminal** is the area where you can see text output from a program.

Python includes `print()` as a built-in function, which means you can use it without defining it yourself.

The `print()` function displays text and other values in the terminal.

## 2. Displaying "Hello World!"

A common first program displays `Hello world!` in the terminal.

You can write this program in Python using the `print()` function.

### Example

    print('Hello world!')

**Output:**

    Hello world!

To do this, place the string `Hello world!` between the opening and closing parentheses of the `print()` function.

For now, consider a **string** as a sequence of characters surrounded by either single (`'`) or double (`"`) quotation marks.

### Another Example

    print("Hello world!")

**Output:**

    Hello world!

Both examples work because Python allows strings to use either single or double quotation marks.

## 3. Understanding Arguments

In the following example:

    print('Hello world!')

The string `'Hello world!'` is an **argument** passed to the `print()` function.

An argument is a value you provide to a function when calling it.

In this example:
- `print()` is the function.
- `'Hello world!'` is the argument.

The function displays the argument in the terminal.

## 4. Printing Multiple Values

You can use the `print()` function to display multiple values at once by separating them with commas.

### Example

    print('My favorite colors are', 'blue', 'green', 'red')

**Output:**

    My favorite colors are blue green red

Python automatically adds a space between items when you separate them with commas.

This is helpful when you want to display several pieces of information together.

### Another Example

    name = 'John'
    age = 25

    print('Name:', name, 'Age:', age)

**Output:**

    Name: John Age: 25

In this example, the `print()` function displays text and variable values together.

## 5. Key Points to Remember

- The terminal displays text output from your program.
- `print()` is a built-in Python function.
- You can use `print()` to display text and other values.
- Strings can be surrounded by single or double quotation marks.
- An argument is a value passed to a function when calling it.
- You can print multiple values by separating them with commas.
- Python automatically adds spaces between items separated by commas in a `print()` call.

## Conclusion

The `print()` function is one of the simplest and most useful functions in Python. It allows you to display messages, variable values, and other information in the terminal.

As you continue learning Python, you will use `print()` to check results, understand how your code behaves, and display information to users.
