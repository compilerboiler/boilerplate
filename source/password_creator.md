---
title: password creator (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'password creator'

Functions in program: 
* `def create_password(n):`

Modules used in program: 
* `import string`
* `import random`

## password creator

Python beginners example: password creator

```python
"""
Why to create strong password?
Because it makes the chances of hackers bruteforcing your password to almost 0%
Simply to not get hacked!
"""

import random
import string

# Password level is Strong!
# Creates a alphanumeric password of `n` chars 
def create_password(n):
    allChars = list(string.ascii_letters) + list(string.digits) + list(string.punctuation)
    passphrase = []
    for i in range(n):
        tmp = random.choice(allChars)
        passphrase.append(tmp)
    
    res = "".join(passphrase)
    return res
    
# Test 1
test1 = create_password(16)
print(test1)

# Test 2 
test2 = create_password(32)
print(test2)


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
