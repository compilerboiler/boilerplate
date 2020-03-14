---
date: 2020-02-16
title: python continue statement
---
---
tags: ["python"]
date: 2020-02-16
title: python continue statement
---
---
tags: ["python"]
date: 2020-02-14
title: python continue statement
---
In [Python](https://python.org) code you can repeat code using loops, the most common being a for loop and a while loop.

Python continue keyword is used to jump out of this cycle, and the [break](https://dev.to/libertycodervice/python-break-statement-4ki5) keyword out of the cycle.

The `continue` statement is used to tell Python to skip the remaining statements in the current cycle, and then proceed with the next cycle.

The continue statement may be used in a [while loop](https://pythonprogramminglanguage.com/while-loop/) and [for loop](https://pythonprogramminglanguage.com/for-loops/).

Python language continue statement syntax is as follows:

```       
    continue
```

## Flow chart:

The control flow graph (flow chart) below shows the continue use:

![python continue statement](https://dev-to-uploads.s3.amazonaws.com/i/knks3huh9rrxwv5r2m7b.jpg)

## Continue Example

The example below uses continue to break out of the cycle, in both the for and while loop.

```python
#!/usr/bin/python

for letter in 'Python': # first instance
   if letter == 'h':
      continue
   print('current letter:', letter)

var = 10 # second instance
while var> 0:
   var = var -1
   if var == 5:
      continue
   print('current variable values:', var)
print("Good bye!")

```

The results of the above examples:

```
current letter: P
current letter: y
current letter: t
current letter: o
current letter: n
current variable values: 9
current variable values: 8
current variable values: 7
current variable values: 6
current variable values: 4
current variable values: 3
current variable values: 2
current variable values: 1
current variable values: 0
Good bye!
```

**Another example**

Python continue statement can be used to skip certain cycle, only the odd-numbered print between 0-10:

```python
#!/usr/bin/python

n = 0
while n <10:
    n = n + 1
    if n% 2 == 0: # If n is even, execute the continue statement
        continue
    print (n)
```
The program outputs:
```
1
3
5
7
9
```

**Related links:**
* [Python book and course](https://gumroad.com/l/dcsp)
* [Python tutorial](https://pythonbasics.org/)

