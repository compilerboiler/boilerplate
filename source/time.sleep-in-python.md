---
tags: ["python"]
date: 2020-02-14
title: time.sleep in python
---
<a href="https://python.org">Python</a> has a module to deal with time. This lets you pause/wait some time in your code. To do this, first import the time module

    #!/usr/bin/python3
    import time

Then you can use the method sleep().

## Pause in Python

To sleep or wait, you can use time.sleep()

    time.sleep(secs)

To sleep for five seconds

    time.sleep(5)

You can also use this to sleep milliseconds

    time.sleep(.500)

Thus, the parameter seconds can be either an integer or floating point number.


## Pause vs threading

To be clear, it pauses the whole program: "Suspend execution of the calling thread". That means that while it is in the sleep method, it does absolutely nothing, not even listen to keyboard or mouse input. 

If you want to do several things at once, look into <a href="https://pythonprogramminglanguage.com/threading/">threading</a>. Every task runs in a thread, so the program could be pausing while still getting keyboard input or receiving to network data.

<img src="https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fpitchenginelive.blob.core.windows.net%2Frefinery%2F28f29690-4305-4640-95e9-c04dab195652%2FGallery%2F4df83d29-aac3-4158-aed7-103e1aa26745.png&f=1&nofb=1" alt="threading">

## How accurate is time.sleep() ?

The sleep method in the Python time module uses the operating systems sleep() function. In other words, the systems sleep code. 

Because operating systems are not accurate like an atomic clock, they have some delay. But don't worry, this delay is usually 1-10 milliseconds and does not matter for 99% of the apps.

**Related links:**

* <a href="http://docs.python.org/3.0/library/time.html">Python time module</a>
* <a href="https://pythonbasics.org/time-and-date/">Time and date in Python</a>
* <a href="https://pythonbasics.org/">Python tutorial</a>
