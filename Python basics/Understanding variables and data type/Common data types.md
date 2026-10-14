# What Are Common Data Types in Python?

Before working with Python variables, it's important to understand data types. A data type describes the kind of value a variable holds, such as a number or a piece of text. Programming languages use data types to determine how to store and work with different kinds of information.

## Dynamic Typing in Python

Python is a dynamically typed language. This means you do not need to specify a variable's data type when creating it. Python determines the type based on the value assigned to the variable.

### Examples

    name = 'John Doe'  # Python knows this is a string
    age = 25           # Python knows this is an integer

A variable can later be assigned a value of a different data type:

    age = 25
    age = 'Twenty-five'

After the second assignment, `age` contains a string instead of an integer.

## Four Common Data Types in Python

For now, focus on these four data types that you will use throughout this module.

### 1. Integer (`int`)

An integer is a whole number without decimal places, such as `10` or `-5`.

    my_integer_var = 10
    print('Integer:', my_integer_var)  # Integer: 10

### 2. Float (`float`)

A float is a number that contains a decimal point, such as `4.41` or `-0.4`.

    my_float_var = 4.50
    print('Float:', my_float_var)  # Float: 4.5

**Note:** Python displays `4.50` as `4.5` because trailing zeros after a decimal point are not necessary when displaying a float.

### 3. String (`str`)

A string is a sequence of characters enclosed in single or double quotation marks, such as `'Hello world!'`.

    my_string_var = 'hello'
    print('String:', my_string_var)  # String: hello

### 4. Boolean (`bool`)

A Boolean represents a truth value. It can be either `True` or `False`.

    my_boolean_var = True
    print('Boolean:', my_boolean_var)  # Boolean: True

## Conclusion

Python has several other data types, but these four are among the most commonly used:

- **Integer (`int`):** Whole numbers.
- **Float (`float`):** Numbers with decimal points.
- **String (`str`):** Text and characters.
- **Boolean (`bool`):** `True` or `False` values.

You will learn about other Python data types as you progress through your programming journey.
