---
date: 2020-02-16
title: python relative import
---
---
tags: ["python"]
date: 2020-02-16
title: python relative import
---
---
tags: ["python"]
date: 2020-02-14
title: python relative import
---
Like any other modern programming language, in <a href="https://python.org">Python</a> you can import code from other files or <a href="https://pythonbasics.org/modules/">modules</a>.  If you used Python before, you know that you can use modules. 

With modules (packages) you can use already existing code bases in your own code, saving you a lot of development time. 

You can import any module with the **import** keyword.

```python
import math
import sys
import os
...
```

Before playing with modules, you should know the <a href="https://pythonbasics.org">basics of Python</a>.

So what is an absolute and a relative import?

## Absolute import

Absolute import defines the resource to be imported by its full path (projects root).  You likely already have used absolute imports, as its the default way of importing modules in Python.

These are examples of absolute imports:

```python
import package
```

And this:

```python
from package.firstmodule import firstmodule
```

## Relative import

A relative import imports the resource relative to the current location. 

In other words, with relative imports you specify *where* your resources are *relative to the current python script*.

```python
# Import names from pkg.string
from .string import name1, name2

# Import pkg.string
from . import string
```

You can see the dot in front of the module, relative imports use dot notation. 

A single dot means the current directory, you may be familiar with this from <a href="https://en.wikipedia.org/wiki/Linux">Linux</a> or command prompt where: 

* dot (.) means current directory
* dot dot (..) means parent directory
* dot dot dot (...) means grandparent directory

## Which to use

You should use absolute imports, unless you have a reason not to. Absolute imports are clear and easy. It specifies where the imported resource is, just by looking at it.

New modules can be <a href="https://pythonbasics.org/how-to-use-pip-and-pypi/">installed with pip</a>, which saves you from having to commit many packages inside your code base.


## Related links
* <a href="https://docs.python.org/2.5/whatsnew/pep-328.html">Python PEP on relative imports</a>
* <a href="https://pythonbasics.org">Learn Python</a>

