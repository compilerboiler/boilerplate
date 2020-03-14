---
date: 2020-02-16
title: python break statement
---
---
tags: ["python"]
date: 2020-02-16
title: python break statement
---
---
tags: ["python"]
date: 2020-02-14
title: python break statement
---
The [Python](https://python.org) break statement, like in C or the C++ programming language, breaks or closes a [for loop](https://pythonprogramminglanguage.com/for-loops/) or a [while loop](https://pythonprogramminglanguage.com/while-loop/).

The `break` statement can be used to terminate a loop statement, i.e., False condition or loop condition has not yet been completed, will stop the execution loop.

The break statement can be used in a while and for loop.

If you are using nested loops, break statement to stop the execution of code gets very confusion, it stops the innermost loop.

**Python language break statement syntax:**
The syntax for the break statement is: (*drum rolls*)
```python   
    break
```
**flow chart:**

![break statement](https://dev-to-uploads.s3.amazonaws.com/i/jrq6oij9bpc383annjgl.jpg)

**Example:**

The example below creates two loops, both which are stopped using the break statement. In the first example we use [strings](https://pythonbasics.org/strings/), in the second example a plain variable counter var.

```python
#!/usr/bin/python
 
for letter in 'Python': # first instance
   if letter == 'h':
      break
   print('current letter:', letter)
  
var = 10 # second instance
while var> 0:
   print('current variable values:', var)
   var = var -1
   if var == 5: # var is equal to 5 when the variable loop exits
      break
 
print("Good bye!")
```
The results of the above examples:
```    
current letter: P
current letter: y
current letter: t
current variable values: 10
current variable values: 9
current variable values: 8
current variable values: 7
current variable values: 6
Good bye!
```
