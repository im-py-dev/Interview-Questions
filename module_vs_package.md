# Python Module vs Package
When working with Python, it is common to come across the terms "module" and "package". Although both of them are used to organize code, there is a fundamental difference between them. In this article, we will explore the differences between a Python module and a package.

## Python Module
A Python module is a single file that contains Python code. It can contain functions, classes, and variables, among other things. Modules are used to organize code into logical units, making it easier to maintain and reuse. You can import a module into your Python script using the import statement.

Here's an example of a simple Python module:

```python
# example.py

def say_hello(name):
    print(f"Hello, {name}!")

class Dog:
    def bark(self):
        print("Woof!")
```

You can import this module into another Python script using the import statement:

```python
# main.py

import example

example.say_hello("John")
my_dog = example.Dog()
my_dog.bark()
```

## Python Package
A Python package, on the other hand, is a collection of one or more Python modules. It is used to organize related code into a single directory hierarchy. A package can have sub-packages, which are packages within packages. A package must contain a special file called __init__.py in its root directory, which can be empty or contain initialization code for the package.

Here's an example of a simple Python package:

```markdown
example_package/
    __init__.py
    module1.py
    module2.py
```

You can import a module from a package using the dot notation:

```python
# main.py

from example_package import module1

module1.say_hello("John")
```

You can also import a package and its modules using the dot notation:

```python
# main.py

import example_package

example_package.module1.say_hello("John")
```

## Conclusion
In summary, a Python module is a single file containing Python code, while a Python package is a collection of one or more Python modules organized into a directory hierarchy.
Modules and packages are used to organize code into logical units, making it easier to maintain and reuse.
