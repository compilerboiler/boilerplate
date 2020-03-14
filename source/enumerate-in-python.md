---
tags: ["python"]
date: 2020-02-16
title: enumerate in python
---
---
tags: ["python"]
date: 2020-02-14
title: enumerate in python
---
Are you new to <a href="https://python.org">Python</a>? Did you program in other languages before?

You may think the way to get the index is by creating a loop, getting the size of the array, creating an index variable, comparing the index variable to the condition and increasing it manually.. phew!

In the C programming language you get something like this:

```c
int i = 0;
for (i = 0; i <= 10; i++){
    printf("%s\n", list[i]);
```

Very cryptic right! 

## For loop index in Python

There is a Pythonic way to create loops with an index, namely **enumerate()**.

```python
for index, value in enumerate(some_list):
    print(index, value)
```

To give you a full example with a <a href="https://pythonbasics.org/list/">list</a>:

```python
my_list = ['apple', 'banana', 'grapes', 'pear']
for c, value in enumerate(my_list):
    print(c, value)

# Output:
# 0 apple
# 1 banana
# 2 grapes
# 3 pear
```
This works for numeric lists too:

```python
>>> b = [3,6,7,2,9]
>>> for index, value in enumerate(b):
...     print(f"At b[{index}] the value is {value}")
... 
At b[0] the value is 3
At b[1] the value is 6
At b[2] the value is 7
At b[3] the value is 2
At b[4] the value is 9
>>>
```

Great right! Syntax is very readable and Pythonic. 

**Related links:**
* <a href="https://pythonbasics.org/enumerate/">More enumerate examples</a>
* <a href="https://gum.co/dcsp">Learn Python, course</a>

