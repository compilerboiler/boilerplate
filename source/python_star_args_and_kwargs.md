---
title: python star args and kwargs (snippet)
date: 2019-02-07
tags: ["python"]
---

## python star args and kwargs

Python beginners example: python star args and kwargs

```python
#!/usr/bin/python

def add_all(*list_of_nums):
  sum = 0
  for num in list_of_nums:
    sum = sum + num
  print('sum ', ' + '.join(str(n) for n in list_of_nums), ' = ', sum)

add_all(2,3,4)

nums = (2,3,4)
add_all(*nums)

nums = [2,3,4]
add_all(*nums)

def add_all_msg(*args, **kwargs):
  print(kwargs['before'])
  add_all(*args)
  print(kwargs['after'])

add_all_msg(2,3,4,before='adding numbers', after='added all numbers')


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
