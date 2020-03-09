---
title: pyqt example setup (snippet)
date: 2020-02-10
tags: ["python"]
---
Python pyqt (gui) example 'setup'


## setup

Python pyqt example: setup

```python
# from distutils.core import setup, Extension
# 
# from Cython.Distutils import build_ext
# 
# 
# setup(
#     cmdclass={'build_ext': build_ext},
#     ext_modules=[Extension("pointtool", sources=[
#                            "pointtool.pyx"], language="c")]
# )

from distutils.core import setup
from Cython.Build import cythonize

setup(
    ext_modules=cythonize("pointtool.pyx"),
)

```

## Useful links

- Learn PyQt: https://pythonbasics.org/pyqt-hello-world/
- Install PyQt: https://pythonbasics.org/install-pyqt/
