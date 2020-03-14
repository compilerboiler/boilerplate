---
date: 2020-02-16
title: stopwatch python
---
---
tags: ["python"]
date: 2020-02-16
title: stopwatch python
---
---
tags: ["python"]
date: 2020-02-14
title: stopwatch python
---
In <a href="https://python.org">Python</a> you can use the time module to wait (you can also get the <a href="https://pythonbasics.org/time-and-date/">time and date</a>). To be explicit, the time module provides various time-related functions.

This is very useful for many applications. If you make a game, it should not update every millisecond. If you make weather station software, it makes no sense to update in such a short time. For an alarm clock app, you need it to wait.

Lets say you want to make a stopwatch, without the program pausing there would be no way to create one.

## Sleep function

The module time has a function named <a href="https://pythonspot.com/sleep/">sleep</a>, which pauses the program (it complete freezes the program).

```python
time.sleep(t)
```

This waits for t number of seconds. Consider this program which waits for one second before it outputs the next word.

```python
import time.sleep

print("Hello")
time.sleep(1)
print("World")
```

## Stopwatch

So you can use the <a href="https://pythonspot.com/sleep/">time.sleep()</a> function to pause the program. But a stopwatch doesn't have a limit, it needs to go on. For that, you can use a <a href="https://pythonbasics.org/while-loop/">while loop</a>. Then you can use Ctrl+c to exit the program.

```python
import time

while True:
    print("Clock ticks")
    time.sleep(1)
```

If you run the above program it outputs:

```bash
➜  ~ python3 stopwatch.py
Clock ticks
Clock ticks
Clock ticks
```

Until you press Ctrl+c. Now it needs to count seconds, you can use time.time() to get the current time.

The example below will output every second passed until Ctrl+C is passed. 

```python
import time

start = time.time()
while True:
    time.sleep(1)
    total_secs = round(time.time() - start)
    print(total_secs)
```

## Formatting

To format it you can use <a href="https://www.python.org/dev/peps/pep-0498/">f-strings</a> with two digits. With a simple calculation you can get the minutes and seconds.

```python
import time

start = time.time()
while True:
    time.sleep(1)
    total_secs = round(time.time() - start)
    minute = round(total_secs / 60)
    seconds = round(total_secs % 60)
    s = f"{minute:02d}:{seconds:02d}"
    print(s)
```

**Related links:**
* <a href="https://docs.python.org/3/library/time.html">The time module</a>
* <a href="https://pythonbasics.org">Learn Python</a>

