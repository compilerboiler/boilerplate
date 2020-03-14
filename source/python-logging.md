---
date: 2020-02-16
title: python logging
---
---
tags: ["python"]
date: 2020-02-16
title: python logging
---
---
tags: ["python"]
date: 2020-02-14
title: python logging
---
You can log in <a href="https://python.org">Python</a> with the logger module. A log file can display or store messages while the program is running.

Logging is very different than just relying on Python errors or <a href="https://pythonbasics.org/try-except/">try-except</a> cases. It is much more broad way to find the bugs in your program.

This is especially useful when your program crashes: it gives you another point of entry to finding the bug. With a large program, you save a lot of time on finding a bug / <a href="https://pythonspot.com/python-debugging/">debugging</a>. 

## Logs

The example below sends a log message to the console.

```python
import logging
logging.warning('this is a warning message')
```

If you run the program it shows:

```bash
➜ python3 example.py 
WARNING:root:this is a warning message
➜   
```

For a slightly larger program:

```python
import logging

x = 2
logging.warning('x associated with value')

y = 3
logging.warning('y associated with value')

z = x / y
logging.warning('calculation complete')
```

Upon running you'll see:

```
➜  python3 example.py 
WARNING:root:x associated with value
WARNING:root:y associated with value
WARNING:root:calculation complete
```

If you set y to zero, you'll see where it stops executing the program:

```bash
WARNING:root:x associated with value
WARNING:root:y associated with value
Traceback (most recent call last):
  File "example.py", line 9, in <module>
    z = x / y
ZeroDivisionError: integer division or modulo by zero
```

Once your program is finished, you can hide logging messages but turn them on when needed by changing the severity level. There are different ways to <a href="https://pythonspot.com/logging/">log messages</a>, like saving the output into a file or adding a timestamp.

**Related links:**
* <a href="https://docs.python.org/3.8/library/logging.html">Documentation on logging</a>
* <a href="https://pythonbasics.org/">Learn Python</a>
