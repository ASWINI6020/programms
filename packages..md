# ABOUT PYTHON PACKGES #
A python package is a collection of modules. Modules that are related to each other are mainly put in the same package. When a module from an external package is required in a program, that package can be imported and its modules can be put to use.Any Python file, whose name is the module’s name property without the .py extension, is a module.A package is a directory of Python modules that contains an additional __init__.py file, which distinguishes a package from a directory that is supposed to contain multiple Python scripts. Packages can be nested to multiple depths if each corresponding directory contains its own __init__.py file.

![Alt text](https://miro.medium.com/max/580/0*Kt5_0uGLlCFAgbt6.png "a title")

# PURPOSE OF PACKAGES #
Use of packages helps importing any modules, individually or whole. While importing a package or sub packages or modules, Python searches the whole tree of directories looking for the particular package and proceeds systematically as programmed by the dot operator
# LIST OF PACKAGES #
There are so many pakages are:
* numpy
* pandas
* Pendulum
* MoviePy
* PyQt
* Pytest
* Pywin32
* Tkinter
* OpenCV Python ........ etc


![Alt text](https://blog.insaid.co/wp-content/uploads/2019/05/10-Python-packages-and-libraries-you-absolutely-have-to-ace.png "a title")

# SIMPLE  PACKAGE EXAMPLE #

![Alt text](https://www.python-course.eu/images/packages_300w.webp "a title")

The content of a.py:

def bar():

    print("Hello, function 'bar' from module 'a' calling")

The content of b.py:

def foo():

    print("Hello, function 'foo' from module 'b' calling")

We will also add an empty file with the name __init__.py inside of simple_package directory
import simple_package from the interactive Python shell, assuming that the directory simple_package is either in the directory from which you call the shell.

from simple_package import a, b

a.bar()

b.foo()

there is a way to automatically load these modules. We can use the file __init__.py for this purpose. All we have to do is add the following lines to the so far empty file __init__.py:

import simple_package.a

import simple_package.b

# SIMPLE PACKAGE CODE #

import simple_package

simple_package.a.bar()

simple_package.b.foo()

# OUTPUT #

Hello, function 'bar' from module 'a' calling

Hello, function 'foo' from module 'b' calling