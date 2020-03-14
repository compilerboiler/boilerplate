---
date: 2020-02-16
title: random number in python
---
In <a href="https://python.org">Python</a> you can generate random numbers with the random module. To load this module use the line

```python
    import random
```

To generate 10 numbers between 1 and 10 you can use:

```python
import random

for x in range(10):
    print(random.randint(1,11))
```

*These are pseudo-random numbers, but for most purposes they are good.*

The lowest possible number here is 1 and the maximum number 10. The for loop is used to repeat this 10 times.

If instead of random integers you want random floats, you can use uniform() as shown in <a href="https://pythonbasics.org/random-numbers/">this example</a>

## Random examples

To get a larger number of random numbers, you can change the for loop. If 
you want 20 numbers use:

```python
import random

for x in range(20):
    print(random.randint(1,11))

```

For 50 numbers use:

```python
import random

for x in range(50):
    print(random.randint(1,11))
```

You get the idea. To get numbers between 1 and 100 you can use:

```python
print(random.randint(1,101))
```

or in a loop

```python
import random

for x in range(50):
    print(random.randint(1,101))
```


**Related links:**
* <a href="https://docs.python.org/3.8/library/random.html">Python documentation on random module</a>
* <a href="https://pythonspot.com/random-numbers/">More random data examples</a>
* <a href="https://pythonspot.com/">Learn Python</a>



