Getting Started with Clint
==========================

``clint`` (Command Line INterface Tools) is a Python package providing
a set of awesome tools for developing command line applications. It
has support for printing in color, indented printing, column printer
and a number of other features. Let's get started.

Installing Clint
----------------

``clint`` is installable via ``pip``. On Fedora Linux, you would do
``sudo pip-python install clint``. 

Printing in color
-----------------
We will explore ``clint's`` feature to print in color in this
section. Consider the following script::

     from clint.textui import colored

     text = 'THIS TEXT IS COLORED %s!'

     if __name__ == '__main__':
         
	 for color in colored.COLORS:
	     rint(getattr(colored, color)(text % color.upper()))


Text Formatting Functions
-------------------------

*Indented printing
*Column printing


Progress bar functionality
--------------------------

Prompting
---------

Argument Parsing
----------------

Working with Pipes
------------------

Configuration files
-------------------



