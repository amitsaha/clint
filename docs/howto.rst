Getting Started with Clint
==========================

``clint`` (Command Line INterface Tools) is a Python package providing
a set of awesome tools for developing command line applications. It
has support for printing in color, indented printing, column printer
and a number of other features. Let's get started.

Installing Clint
----------------

``clint`` is installed via ``pip``. On Fedora Linux, you would do
``sudo pip-python install clint``. 

Printing in color
-----------------
We will explore ``clint's`` feature to print in color in this
section. Consider the following example::

     >>> from clint.textui import puts, colored
     >>> puts(colored.red('Text in Red'))
     Text in Red 

Note that the above text is in ``red``. Likewise, you can use the
other colors. Consider the next script::

     #!/usr/bin/env python
     # Print text in all colors

     from clint.textui import colored, puts

     if __name__ == '__main__':
        for color in colored.COLORS:
                 puts(getattr(colored,color)('Text in {0:s}'.format(color.upper()))

This script produces the following output::

     Text in RED
     Text in GREEN
     Text in YELLOW
     Text in BLUE
     Text in BLACK
     Text in MAGENTA
     Text in CYAN
     Text in WHITE


Indented printing
-----------------
Let's say you want to print indented text. Its simple with ``clint``:

Column printing
---------------


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



