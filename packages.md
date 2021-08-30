# ABOUT PYTHON PACKGES 
A python package is a collection of modules. Modules that are related to each other are mainly put in the same package. When a module from an external package is required in a program, that package can be imported and its modules can be put to use.Any Python file, whose name is the module’s name property without the .py extension, is a module.A package is a directory of Python modules that contains an additional __init__.py file, which distinguishes a package from a directory that is supposed to contain multiple Python scripts. Packages can be nested to multiple depths if each corresponding directory contains its own __init__.py file.

![Alt text](https://www.mediaan.com/wp-content/uploads/2021/02/Header-Python-Packages-Blog-Final-Image.jpg "a title")

# PURPOSE OF PACKAGES 
Use of packages helps importing any modules, individually or whole. While importing a package or sub packages or modules, Python searches the whole tree of directories looking for the particular package and proceeds systematically as programmed by the dot operator

# LIST OF PACKAGES #
There are so many pakages are:
* numpy
* pandas 
* pendulum
* MoviePy
* PyQt
* Pytest
* Pywin32
* Tkinter
* OpenCV Python ...etc

![Alt text](https://blog.insaid.co/wp-content/uploads/2019/05/10-Python-packages-and-libraries-you-absolutely-have-to-ace.png "a title")

# numpy
numpy is used as  basic mathematical operations without any special Python packages. However, if you’re going to do any kind of complex math, the NumPy package will make your coding life much easier.NumPy provides tools to help build multi-dimensional arrays and perform calculations on the data stored in them. You can solve algebraic formulas, perform common statistical operations, and much more. 

![Alt text](https://static.javatpoint.com/tutorial/numpy/images/numpy-tutorial.png "a title")
 
# pandas
Python packages designed for working with complex data sets. But arguably, Pandas is the most important. Pandas helps you manipulate and analyze large sets of data without having to learn a specialized data-processing language like R.Pandas has its limits in that it’s not intended for advanced statistical modelling.

![Alt text](https://okfnlabs.org/img/posts/pandas_logo.png "a title")

# pendulum
Pendulum Python package makes it easier to do more complex coding involving dates and times. It’s more intuitive to work with, and it manages time zones automatically. Pendulum is designed to be a drop-in replacement for datetime. That means you can use it with code you’ve already written based on datetime. With only a few exceptions, Pendulum will work just as well, without the need to modify the code, while providing extra features not present in plain-old datetime.
 
# MoviePy
MoviePy is to videos what Pillow is to images. It provides a range of functionality for common tasks associated with importing, modifying, and exporting video files. It also lets you do things like insert titles into videos or rotate videos 90 degrees.MoviePy is not intended as a tool for advanced data manipulation. If you’re writing a video editing app, you’ll probably also need to rely on OpenCV.

![Alt text](https://codingdeekshi.com/wp-content/uploads/2021/07/Convert-Mp4-Video-to-Mp3-Audio-Python-Moviepy-Script-pic.jpg "a title")
 
# PyQt
The preceding sentence notwithstanding, PyQT, another Python package for building GUIs, is also a strong contender. It provides bindings to (you guessed it) the Qt toolkit, which is also cross-platform. It’s intended for heavier-duty GUI programming than Tkinter. That means that PyQT may be overkill if you’re building an app that has a pretty simple interface — say, just a window with some buttons and text fields

# Pywin32
Pywin32 is a must-have package. It provides access to many of the native Windows API functions, allowing you to do things like interact with the Windows registry, use the Windows clipboard, and much more.

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