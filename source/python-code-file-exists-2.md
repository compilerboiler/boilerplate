---
title: python-code-file-exists-2 (snippet)
date: 2020-02-15
tags: ["python"]
---
Python example 'python-code-file-exists-2'


Modules used in program: 
* `import os `

## python-code-file-exists-2

Python code example: python-code-file-exists-2

```python

# Leverage the OS package (possible race condition)
import os 
exists = os.path.isfile('/path/to/file')

# Wrap the path in an object for enhanced functionality
from pathlib import Path
config = Path('/path/to/file') 
if config.is_file(): 
  pass


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org

More Python: https://pythonprogramminglanguage.com
