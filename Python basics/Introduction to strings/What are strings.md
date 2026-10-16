# What Are Strings and What Is String Immutability?

## 1. What Is a String?

A **string** is a sequence of characters surrounded by either single or double quotation marks. Python treats both forms as strings, so you can use either one.

### Example

    my_str_1 = 'Hello'
    my_str_2 = "World"

## 2. Multiline Strings

If you need a multiline string, you can use triple double quotes (`"""`) or triple single quotes (`'''`).

### Example

    my_str_3 = """Multiline string"""
    my_str_4 = '''Another multiline string'''

These quotation marks allow you to create strings that span multiple lines.

### Example

    message = """Hello
    Welcome to Python
    Keep learning!"""

    print(message)

**Output:**

    Hello
    Welcome to Python
    Keep learning!

## 3. Strings Containing Quotation Marks

If your string contains either single or double quotation marks, you have two options.

### Method 1: Use the Opposite Kind of Quotes

If your string contains single quotes, use double quotes to wrap the string, and vice versa.

**Example:**

    msg = "It's a sunny day"
    quote = 'She said, "Hello World!"'

In this example:
- The variable `msg` uses double quotes because the string contains a single quote.
- The variable `quote` uses single quotes because the string contains double quotes.

### Method 2: Escape the Quotation Marks

You can escape a single or double quotation mark in a string using a backslash (`\`).

**Example:**

    msg = 'It\'s a sunny day'
    quote = "She said, \"Hello!\""

The backslash tells Python to treat the quotation mark as part of the string rather than as the end of the string.

## 4. Checking Whether a String Contains Certain Characters

Python provides the **`in` operator**, which returns a Boolean indicating whether the specified character or characters exist in the string.

### Example

    my_str = 'Hello world'

    print('Hello' in my_str)  # True
    print('hey' in my_str)    # False
    print('hi' in my_str)     # False
    print('e' in my_str)      # True
    print('f' in my_str)      # False

**Output:**

    True
    False
    False
    True
    False

### Explanation

- `'Hello' in my_str` returns `True` because `'Hello'` exists in the string.
- `'hey' in my_str` returns `False` because `'hey'` does not exist in the string.
- `'hi' in my_str` returns `False` because `'hi'` does not exist in the string.
- `'e' in my_str` returns `True` because the character `'e'` exists in the string.
- `'f' in my_str` returns `False` because the character `'f'` does not exist in the string.

**Remember:** Python's string searches are case-sensitive. For example, `'hello'` and `'Hello'` are different strings.

## 5. Getting the Length of a String

To get the length of a string, you can use Python's built-in **`len()` function**.

The `len()` function returns the number of characters in a string, including spaces and punctuation.

### Example

    my_str = 'Hello world'

    print(len(my_str))  # 11

**Output:**

    11

The string `'Hello world'` contains 11 characters, including the space between the two words.

## 6. String Indexing

Each character in a string has a position called an **index**.

Python uses zero-based indexing, meaning:

- The first character has an index of `0`.
- The second character has an index of `1`.
- The third character has an index of `2`.
- The pattern continues for the remaining characters.

To access a character by its index, use square brackets (`[]`) with the index of the character you want to access inside.

### Example

    my_str = "Hello world"

    print(my_str[0])  # H
    print(my_str[6])  # w

**Output:**

    H
    w

### Understanding the Index Positions

For the string `"Hello world"`:

| Character | Index |
|---|---:|
| H | 0 |
| e | 1 |
| l | 2 |
| l | 3 |
| o | 4 |
| Space | 5 |
| w | 6 |
| o | 7 |
| r | 8 |
| l | 9 |
| d | 10 |

Therefore, `my_str[0]` returns `'H'`, while `my_str[6]` returns `'w'`.

## 7. Negative Indexing

Python also allows **negative indexing**, which lets you access characters starting from the end of a string.

- `-1` accesses the last character.
- `-2` accesses the second-to-last character.
- `-3` accesses the third-to-last character.

### Example

    my_str = 'Hello world'

    print(my_str[-1])  # d
    print(my_str[-2])  # l

**Output:**

    d
    l

Negative indexing is useful when you want to access characters from the end of a string without knowing its length.

## 8. What Are Mutable and Immutable Values?

In Python, values can be **mutable** or **immutable**.

### Mutable Values

A mutable value can be changed after it is created.

For example, lists are mutable:

    my_list = [1, 2, 3]

    my_list[0] = 10

    print(my_list)  # [10, 2, 3]

Here, we changed the first element of the list from `1` to `10`.

### Immutable Values

An immutable value cannot be changed after it is created.

Strings are immutable in Python.

This means you cannot directly add, remove, or replace individual characters in an existing string.

However, you can point a variable at a new value. This is called **reassignment**.

## 9. String Immutability

Strings are immutable in Python, but you can still reassign a variable to a different string.

### Example: Reassigning a String

    greeting = 'hi'

    greeting = 'hello'

    print(greeting)  # hello

**Output:**

    hello

### Explanation

First, the variable `greeting` refers to the string `'hi'`.

Then, we reassign `greeting` to the string `'hello'`.

This is allowed because we are not modifying the original string. We are making the variable refer to a different string.

## 10. Trying to Modify a String Directly

Although reassignment is allowed, directly modifying an individual character in a string is not allowed.

### Example

    greeting = 'hi'

    greeting[0] = 'H'

**Output:**

    TypeError: 'str' object does not support item assignment

### Explanation

The expression:

    greeting[0] = 'H'

attempts to replace the first character of the string `'hi'` with `'H'`.

Python raises a `TypeError` because strings are immutable.

### How Can You Create a Modified String?

Instead of modifying the original string, you can create a new string:

    greeting = 'hi'

    greeting = 'H' + greeting[1:]

    print(greeting)  # Hi

**Output:**

    Hi

Here, Python creates a new string, `'Hi'`, and assigns it to `greeting`.

The original string was not modified.

## 11. Other Immutable Data Types

Strings are not the only immutable values in Python.

**Integers, floats, and Booleans are also immutable.**

### Example

    age = 20          # Integer
    price = 19.99     # Float
    is_active = True  # Boolean

You can reassign these variables to different values, but you cannot modify the original values themselves.

You will learn about other immutable types in later lessons.

## Quick Summary

| Concept | Meaning |
|---|---|
| String | A sequence of characters enclosed in quotation marks. |
| Single quotes | Used to create strings, such as `'Hello'`. |
| Double quotes | Used to create strings, such as `"Hello"`. |
| Triple quotes | Used for multiline strings. |
| Escape character (`\`) | Allows special characters, such as quotation marks, to be included in a string. |
| `in` operator | Checks whether a character or substring exists in a string. |
| `len()` | Returns the number of characters in a string. |
| Indexing | Accesses a character using its position. |
| Negative indexing | Accesses characters from the end of a string. |
| Mutable | A value that can be changed after creation. |
| Immutable | A value that cannot be changed after creation. |
| Reassignment | Assigning a variable to a new value. |
| String immutability | The inability to modify individual characters of an existing string. |
