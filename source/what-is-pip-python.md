---
tags: ["python"]
date: 2020-02-14
title: what is pip python
---
In the <a href="https://python.org">Python</a> programming languages, you can use code of others, packages. PIP is a package manager for Python <a href="https://pythonbasics.org/modules/">modules</a>. Modules are Python code libraries you can include in your project. 

For Python > 3.4 pip is installed by default.
Is pip installed? You can check with this command:

    ➜ pip --version

or the command

    ➜ pip3 --version

If it's not installed, you can run this command (on Linux)

    ➜  ~ sudo apt install python3-pip

If you don't use Linux, check these <a href="https://pypi.org/project/pip/">pip download</a>.

# Install module

You can install a module with the line (pip3 install <module>), the example below installs a package. You may need pip install of pip3.

```python
➜  ~ pip3 install camelcase      
Collecting camelcase
  Downloading https://files.pythonhosted.org/packages/24/54/6bc20bf371c1c78193e2e4179097a7b779e56f420d0da41222a3b7d87890/camelcase-0.2.tar.gz
Building wheels for collected packages: camelcase
  Running setup.py bdist_wheel for camelcase ... done
  Stored in directory: /home/frank/.cache/pip/wheels/b1/fe/08/84d2143069bc44c20127c38cc1bf202332319b3da7315ca766
Successfully built camelcase
Installing collected packages: camelcase
Successfully installed camelcase-0.2
➜  ~ 
```

You can use that module once installed. Just type import <modulename> and then use it:

```python
➜ python3
Python 3.7.5 (default, Nov 20 2019, 09:21:52) 
[GCC 9.2.1 20191008] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import camelcase
>>> c = camelcase.CamelCase()
>>> print(c.hump("hello"))
Hello
>>> 
```

**Related links:**
* <a href="https://pypi.org/project/pip/">Python package manager</a>
* <a href="https://pythonbasics.org">Learn Python</a>
