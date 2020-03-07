---
title: python  compiler (snippet)
date: 2019-02-07
tags: ["python"]
---

## python  compiler

Python beginners example: python  compiler

```python
from cx_Freeze import setup, Executable

# file must be saved in same directory as the file you want to Compile
# Download cx_Freeze from source forge or run easy_install in power shell

nameOfExec = input("Name for Executable: ")
versionNumber = input("Version: ")
auth = input("Name of Author: ")
auth_email = input("Email of Author: ")
descript = input("Description: ")
filename = input("File to Compile(Add .py to file): ")

# run this file in cmd "python CompileFiles.py build" or "python CompileFiles.py build_exe"
# This setup in minimialistic

setup(
    name = nameOfExec,
    version = versionNumber,
    description = descript, 
    author = auth,
    author_email = auth_email,
    executables = [Executable(filename)]
    )


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
