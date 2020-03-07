---
title: in the something (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'in the something'


Modules used in program: 
* import random

## in the something

Python beginners example: in the something

```python
import random

# "The something in something" program
noun_lib = ["cat","dog","lizard","bald","insane guy","CEO","monkey","teacher","ballerina","old man","nerd","lion","alien","elephant"]
place_lib = ["in Hungary","in the toilet","in a car","in a zoo","in a lions cave","in a park","in Norway","in Rio","on Mars","on a tree","on the roof of Burj-Khalifa"]

flag = True
while flag:
    inp = str(input("\nDo you want more? [Y/n] "))
    if inp.strip().lower() == "y":
        print("-> The" + " " + random.choice(noun_lib) + " " + random.choice(place_lib) + ".")
    else:
        flag = False


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
