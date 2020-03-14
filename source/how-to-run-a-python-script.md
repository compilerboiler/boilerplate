---
date: 2020-02-16
title: how to run a python script
---
Before writing <a href="https://python.org">Python</a> scripts, you should be able to run them. If you run a Python script, Python makes sure the computer understands the code: it interprets. 

Any Python script should end with the .py extension. So program names could be:

* hello.py
* world.py
* sort_names.py

The way to execute Python differs on systems (Linux,Mac,Windows), but comes down to the same idea. Any script will do, you can use the <a href="https://pythonbasics.org/execute-python-scripts/">hello world</a> script.

## Windows

On Windows, you likely installed Python in C:\Python..\python.exe
But your program is most probably somewhere else, like on your desktop. 
First open a command prompt (Win+R, cmd or command.exe)
You can run it with this command:

    C:\Python35\python.exe C:\Users\Username\Desktop\my_python_script.py

On older versions of windows, Python is not installed by default. If that's the case, install it first.

## On Mac OS X or Linux

If you use Apple Mac or Linux, Python is often installed by default. On top of the program, you can add one of these lines:

    #!/usr/bin/env python

or

    #!/usr/bin/env python3

This defines that you want to use Python environment. Save your file (hello.py).

Then in the command line, make it executable:

    chmod +x hello.py

Then you can run it like any other program. An alternative is to run it with the python interpreter:
```python
    python hello.py
```
## Alternatives

Working from the command line can be quite challenging. For a single file you can do it, but for larger apps this gets cumbersome.

Most developers use an app to develop, a so called <a href="https://pythonbasics.org/getting-started/#PythonIDE">IDE</a>. This lets you work with multiple files easily, run with a keyboard shortcut and other simplifications.

![Alt Text](https://dev-to-uploads.s3.amazonaws.com/i/z9lzs3l610rirsb903f7.jpeg)

Sometimes people work directly in the Python shell, sometimes named <a href="https://pythonprogramminglanguage.com/repl/">REPL</a>. This lets you interact with Python, but doesn't require a file.

To open the Python shell, you simply type 'python' in the command prompt. That sets you into the shell.

    ➜  ~ python3
    Python 3.7.5 (default, Nov 20 2019, 09:21:52) 
    [GCC 9.2.1 20191008] on linux
    Type "help", "copyright", "credits" or "license" for more information.
    >>> 
 
To exit the shell, press Ctrl+Z.

**Related links:**
* <a href="https://python.org/">Python language homepage</a>
* <a href="https://pythonbasics.org/">Python tutorial</a>



