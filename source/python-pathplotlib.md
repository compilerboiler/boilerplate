---
date: 2020-02-16
title: python pathplotlib
---
With the <a href="https://python.org">Python</a> programming language, you can deal with files. Some things you can do with Python are <a href="https://pythonbasics.org/read-file/">read files</a>, <a href="https://pythonbasics.org/write-file/">write files</a>, create files and much more. 

If you worked with files in Python, you know that dealing with Paths can be quite cumbersome. On top of that paths are written differently on systems like Windows (\) or Mac (/)

You may be familiar with having to deal with double slashes and the like:

```python
b = "c:\\stuff\\morestuff\\furtherdown\\THEFILE.txt"
```

Meet the <a href="https://docs.python.org/3/library/pathlib.html">pathlib</a> module, which prevents you from writing code like this.

## Pathlib

Pathlib makes working with paths and files in general easier. Instead of those ugly double slashes you can write elegant and readable Python code. 
To get your home directory:

```python
>>> import pathlib
>>> pathlib.Path.home()
```

The current working directory:

```python
>>> import pathlib
>>> pathlib.Path.cwd()
```

You can simply add slashes for subdirectories

```python
>>> pathlib.Path.home() / 'Desktop' / 'pama'
```

To define a filepath you can do this:

```python
>>> filename = pathlib.Path.home() / 'Desktop' / 'files' / 'test.txt'
>>> filename
```

So you can use that path (filename) to read files as you would normally do:

```python
>>> filename = pathlib.Path.home() / 'rdp.txt'
>>> with open(filename, mode='r') as f:
...     data = f.readlines()
... 
>>> data
```

You can even read files with one liner:

```python
data = pathlib.Path(pathlib.Path.home() / 'rdp.txt').read_text()
```

To get the extension, name or parent of a path is also super easy:

```python
>>> path = pathlib.Path.home() / 'Desktop' / 'files' / 'test.txt'
>>> path.name
'test.txt'
>>> path
PosixPath('/home/tux/Desktop/files/test.txt')
>>> path.parent
PosixPath('/home/tux/Desktop/files')
>>> path.suffix
'.txt'
>>> path.stem
'test'
>>>
```

**Related links:**
* <a href="https://docs.python.org/3/library/pathlib.html">Python Pathlib module</a>
* <a href="https://pythonbasics.org/">Learn Python</a>
