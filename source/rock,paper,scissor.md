---
title: rock,paper,scissor (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'rock,paper,scissor'. This lets you play the little game 'rock, paper, scissor' in Python.

Modules used in program: 
* `import random`

## rock,paper,scissor

Python beginners example: rock,paper,scissor

```python
import random
while 2 == 2:
    print('--------------------------------------------------------------')
    get_again = raw_input('Enter rock paper or scissor :  ')
    make_use = random.choice(['rock','paper','scissor'])
    print('--------------------------------------------------------------')
    print(make_use)
    print('--------------------------------------------------------------')
    if get_again == 'rock' and make_use == 'paper':
        print('computer wins! You "LOSE" ')
        print('--------------------------------------------------------------')
        continue
    elif get_again == 'rock' and make_use == 'scissor':
        print('computer loses You win!')
        print('--------------------------------------------------------------')
        break
    elif get_again == 'rock' and make_use == 'rock':
        print('It\'s a tie ! try again !')
        print('--------------------------------------------------------------')
        continue
    elif get_again == 'paper' and make_use == 'paper':
        print('It\'s a tie ! try again !')
        print('--------------------------------------------------------------')
        continue
    elif get_again == 'scissor' and make_use == 'scissor':
        print('It\'s a tie ! try again !')
        print('--------------------------------------------------------------')
        continue
    elif get_again == 'paper' and make_use == 'scissor':
        print('computer wins! You "LOSE" ')
        print('--------------------------------------------------------------')
        continue
    elif get_again == 'scissor' and make_use == 'paper':
        print('computer loses You win!')
        print('--------------------------------------------------------------')
        break
    elif get_again == 'paper' and make_use == 'rock':
        print('computer wins! You "LOSE" ')
        print('--------------------------------------------------------------')
        continue
    elif get_again == 'scissor' and make_use == 'rock':
        print('computer wins You "LOSE" ')
        print('--------------------------------------------------------------')
        continue
    else :
        print('Invalid input: Try again')
        continue

    


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
