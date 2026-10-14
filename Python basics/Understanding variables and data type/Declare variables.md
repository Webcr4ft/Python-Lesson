# How Do You Declare Variables and What Are Naming Conventions to Name Variables?

## 1. Declaring Variables

In Python, variables are like labeled boxes for storing and referencing data of different types.

To create a variable, write its name on the left, followed by the assignment (`=`) operator and the value you want to store on the right.

### Example

    name = 'John Doe'
    age = 25

In the example above:
- `name` is a variable that holds the value `'John Doe'`.
- `age` is a variable that holds the value `25`.

The value `'John Doe'` is a **string**, which is a series of characters used to represent text.

Strings can be written using single or double quotation marks:

    name = 'John'
    greeting = "Hello"

In future lessons, you'll learn more about working with strings in Python.

## 2. Following Naming Rules

When naming variables in Python, there are some important rules you should keep in mind.

### Rule 1: Variable Names Cannot Start With a Number

Variable names must start with a letter or an underscore (`_`), not a number.

**Valid examples:**

    name = "John"
    _age = 25
    age2 = 30

**Invalid example:**

    5variable_name = 5

This raises a `SyntaxError` because a variable name cannot begin with a number.

### Rule 2: Variable Names Can Only Contain Specific Characters

Variable names can contain:
- Lowercase letters (`a-z`).
- Uppercase letters (`A-Z`).
- Numbers (`0-9`), provided the name does not start with a number.
- Underscores (`_`).

**Valid examples:**

    user_name = "John"
    age2 = 25
    total_price = 100

**Invalid examples:**

    user-name = "John"
    total price = 100

Hyphens and spaces are not allowed in variable names.

### Rule 3: Variable Names Are Case-Sensitive

Python treats uppercase and lowercase letters as different characters.

For example:

    age = 20
    Age = 25
    AGE = 30

These are three different variables.

### Rule 4: You Cannot Use Python's Reserved Keywords

Python has reserved keywords that serve specific purposes in the language.

Examples include:
- `if`
- `class`
- `def`
- `for`
- `while`
- `return`

You cannot use these keywords as variable names.

**Invalid example:**

    class = "Python"

This raises a `SyntaxError` because `class` is a reserved keyword.

**Valid alternative:**

    class_name = "Python"

## 3. Following Naming Conventions

Naming rules determine whether a variable name is valid, while naming conventions are recommended practices that make code easier to read and maintain.

### Convention 1: Use Snake Case

Python variable names should generally be written in lowercase, with words separated by underscores (`_`).

This naming style is called **snake_case**.

**Example:**

    my_variable_name = "freeCodeCamp"

Another example:

    total_price = 500
    user_age = 30

Snake case makes variable names easier to read, especially when they contain multiple words.

### Convention 2: Use Descriptive Variable Names

You should use descriptive names that explain what a variable represents.

For example, if you want to store a user's age, `user_age` is more descriptive than `age` or an abbreviation like `ua`.

**Example:**

    user_age = 30

Descriptive names help you and other developers understand your code, especially when working on large projects.

### Convention 3: Avoid Unclear Single-Letter Variable Names

Single-letter variable names are sometimes used in Python, but they should generally be avoided when they make the code difficult to understand.

**Example:**

    x = 56

The name `x` does not explain what the value represents.

A more descriptive name would be:

    product_price = 56

However, single-letter names such as `i` and `j` are commonly used for loop counters, where their purpose is clear from the context.

## 4. Writing Comments

Comments allow you to add notes and explanations to your code.

In Python, comments start with the pound symbol (`#`). Python ignores everything after the `#` symbol on that line.

### Single-Line Comments

**Example:**

    # This is a single-line comment

You can also place a comment after a line of code:

    age = 25  # Stores the user's age

### Multi-Line Comments

You can create a multi-line comment by using consecutive single-line comments.

**Example:**

    # This is a comment
    # that spans multiple
    # lines

Comments can help you:
- Explain complicated parts of your code.
- Leave reminders for yourself.
- Clarify why a particular piece of code exists.
- Help other developers understand your code.

Comments are especially helpful when learning programming or working with a team.

### Avoid Using Comments to Explain Unclear Variable Names

You should not rely on comments to explain what an unclear variable name means. Instead, choose a descriptive name that communicates its purpose.

**Less clear:**

    x = 56  # This is the product price

**Better:**

    product_price = 56

The second example is easier to understand because the variable name explains what the value represents.

## Conclusion

When declaring variables in Python, use the assignment (`=`) operator to store values under variable names.

Remember these key points:

- Variable names must start with a letter or an underscore, not a number.
- Variable names can contain letters, numbers, and underscores.
- Variable names are case-sensitive.
- Reserved keywords cannot be used as variable names.
- Use snake_case for variable names.
- Choose descriptive names that explain what the variables represent.
- Use comments to explain your code when necessary.

**Following these rules and conventions will help you write Python code that is readable, organized, and easier to maintain.**
