---
title: magicball 8 (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'magicball 8'

Functions in program: 
* `def magic():`

Modules used in program: 
* import random

## magicball 8

Python beginners example: magicball 8

```python
import random

def magic():
    input("Ask me a question . Try me: ")
    return random.choice([ "It is certain" , "Outlook good" , "You may rely on it" , "Ask again later" , "Concentrate and ask again" , "Reply hazy, try again" , "My reply is no" , "My sources say no" ])

# main Sector
print("Hello,")
while True:
    if input("start or end: ").strip().lower() == "start":
        print(magic(), "\n")
        continue
    else:
        quit()


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
