---
date: 2020-02-16
title: python get files in directory
---
---
tags: ["python"]
date: 2020-02-16
title: python get files in directory
---
---
tags: ["python"]
date: 2020-02-14
title: python get files in directory
---
How do you get the filenames in a directory? You can do that automatically with <a href="https://python.org/">Python</a>, including all files in sub directories.

To get started, you need to import the os module, this contains operating system specific functionality.

In Python, you can use OS.walk(). OS.walk() gets the filenames in a directory. It does so by walking the <a href="https://pythonspot.com/python-tree/">tree</a> either top-down or bottom-up.

You should know the <a href="https://pythonbasics.org">basics of Python</a> or this will be a bit confusing.

## OS.walk()

Calling the OS.walk() method returns a 3-<a href="https://pythonspot.com/python-tuples/">tuple</a> (dirpath, dirnames, filenames).

```python
os.walk(top, topdown=True, onerror=None, followlinks=False)
```

* *dirpath* is a string, the path to the directory. 
* *topdown* is an optional argument
* *onerror* is an optional argument, by default errors are ignored
* *followlinks* is false will not walk down into symbolic links that resolve to directories

The function returns lists for dirnames and filesnames, so you can use a <a href="https://pythonbasics.org/for-loops/">for loop</a> to parse it.

To output the files in a directory you can run the code below:

```python
import os

for root, dirs, files in os.walk("/etc/"):
    for name in files:
        print( root + "/" + name)
```

This outputs all files in the directory, including sub-directories. To get all sub directories you can just change files to dirs:

```python
import os

for root, dirs, files in os.walk("/etc/"):
    for name in dirs:
        print( root + "/" + name)
```

You can get the file size too:

```python
import os
from os.path import join, getsize
from pathlib import Path

# needs Python 3.5+
home = str(Path.home())

for root, dirs, files in os.walk(home + "/Desktop/"):
    print(root, "consumes", end=" ")
    print(sum(getsize(join(root, name)) for name in files), end=" ")
    print("bytes in", len(files), "non-directory files")
```

I've used this line to get the home directory in Python 3.5:

```python
from pathlib import Path
home = str(Path.home())
```

If you have an older Python version you can use

```python
from os.path import expanduser
home = expanduser("~")
```

**Related links:**
* <a href="https://docs.python.org/3/library/os.html">Python os module</a>
* <a href="https://pythonbasics.org/">Learn Python</a>
