# How Do the `type()` and `isinstance()` Functions Work?

In the previous lesson, you learned about common data types in Python, including strings, integers, and floats. As you build your programs, you will need to learn how to check the type of a variable.

## The `type()` Function

Here is an example variable:

    developer = 'Devin'

To see the type of `developer`, you can use the `type()` function like this:

    developer = 'Devin'

    print(type(developer))  # <class 'str'>

The output `<class 'str'>` means that `developer` is a string.

If you fail to provide the required arguments to the `type()` function, you will receive an error message:

    Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
    TypeError: type() takes 1 or 3 arguments

### Checking Different Data Types

Here are the data types you have learned so far, along with what the `type()` function prints for each one:

    my_integer_var = 10
    print(type(my_integer_var))  # <class 'int'>

    my_float_var = 4.50
    print(type(my_float_var))  # <class 'float'>

    my_string_var = 'hello'
    print(type(my_string_var))  # <class 'str'>

    my_boolean_var = True
    print(type(my_boolean_var))  # <class 'bool'>

## The `isinstance()` Function

There will be times in your programs when you need to verify that a particular variable is a specific type before performing operations on it. This is where the `isinstance()` function comes in handy.

Here is an example variable with a string assigned to it:

    account_balance = '12'

If you try to perform mathematical operations, such as division, using the `account_balance` variable, you will receive an error message.

    account_balance = '12'

    account_balance / 2

    # Traceback (most recent call last):
    #   File "<stdin>", line 1, in <module>
    # TypeError: unsupported operand type(s) for /: 'str' and 'int'

### Checking a Variable's Type

To see if `account_balance` is an integer, you can use the `isinstance()` function like this:

    account_balance = '12'

    isinstance(account_balance, int)  # False

The built-in `isinstance()` function lets you check whether a variable matches a specific data type. It takes a value and the type you want to check it against, then returns a Boolean (`True` or `False`).

In this case, since `account_balance` is a string, the function returns `False`.

### Checking Multiple Data Types

The `isinstance()` function also allows you to check for multiple types at once.

Here is an example checking whether `account_balance` is an integer or a float:

    account_balance = 12

    isinstance(account_balance, (int, float))  # True

In this example, `account_balance` is an integer, so `isinstance()` returns `True`.

If `account_balance` were `12.0`, `isinstance()` would still return `True` because you are checking for either integers or floats.

## Conclusion

The `type()` and `isinstance()` functions help you work with data types in Python.

- **`type()`:** Identifies the type of a value or variable.
- **`isinstance()`:** Checks whether a value belongs to a specified data type or types and returns `True` or `False`.

In future workshops and labs, you will use these functions to ensure your variables contain the correct data types before performing operations on them.
