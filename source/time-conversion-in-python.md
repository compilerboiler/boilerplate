---
tags: ["python"]
date: 2020-02-16
title: time conversion in python
---
---
tags: ["python"]
date: 2020-02-14
title: time conversion in python
---
In Python, the <a href="https://docs.python.org/3.8/library/time.html">time</a> module provides many time related functions. 

You can use the time module to get the <a href="https://pythonbasics.org/time-and-date/">time and date</a> and other things. You can use the function *time.time()* to get get the current time

```python
import time

time.time()
```

But if you output it with the print function, it doesn't show in human readable format. Instead you get a number called the <a href="https://en.wikipedia.org/wiki/Unix_time">epoch</a> or Unix time. 

<img src="https://duckduckgo.com/i/aa977c6c.jpg" alt="unix time">

This is a system for describing a point in time that is used by computers. So how do you convert it to time?

Before playing with time module, you should know the <a href="https://pythonbasics.org">basics of Python</a>.

## ctime

One way to solve this is by calling the function ctime(). The ctime() function converts a time (seconds since the <a href="https://en.wikipedia.org/wiki/Unix_time">epoch</a>) to a string of a form: 'Sun Jun 20 23:21:05 1993'.

```python
import time

now = time.ctime(int(time.time()))
print(now)
```

The program shows the current date and time:

```
Thu Feb 13 14:00:03 2020
```

## strftime

To get just the time you can use the function strftime(). This outputs hours "%H" and minutes "%M". To get the seconds you can use "%S". Try the code:

```python
import time

now = time.strftime("%H:%M", time.localtime(time.time()))
print(now)
```

## alternative

To convert the time manually to hours, seconds and minutes you can do the math manually. Then use <a href="https://www.python.org/dev/peps/pep-0498/">f-strings</a> to output 2 digits for every variable:

```python
import time

time = time.time()
time = time % (24 * 3600)
hour = round(time // 3600)
time %= 3600
minutes = round(time // 60)
time %= 60
seconds = round(time)

print(f"{hour:02d}:{minutes:02d}:{seconds:02d}")
```

This returns the nicely formatted time:

```
$ python example.py
13:06:29
```


**Related links:**
* <a href="https://docs.python.org/3.8/library/time.html">Time module for Python 3</a>
* <a href="https://pythonbasics.org">Learn Python</a>

