---
title: python code sum elements two lists (snippet)
date: 2020-02-15
tags: ["python"]
---
Python example 'python code sum elements two lists'


Modules used in program: 
* `import numpy as np `
* `import operator `

## python code sum elements two lists

Python code example: python code sum elements two lists

```python
ethernet_devices = [1, [7], [2], [8374163], [84302738]]
usb_devices = [1, [7], [1], [2314567], [0]]

# The long way
all_devices = [
  ethernet_devices[0] + usb_devices[0], 
  ethernet_devices[1] + usb_devices[1], 
  ethernet_devices[2] + usb_devices[2], 
  ethernet_devices[3] + usb_devices[3], 
  ethernet_devices[4] + usb_devices[4]
]

# Some comprehension magic
all_devices = [x + y for x, y in zip(ethernet_devices, usb_devices)]

# Let's use maps
import operator 
all_devices = list(map(operator.add, ethernet_devices, usb_devices))

# We can't forget our favorite computation library
import numpy as np 
all_devices = np.add(ethernet_devices, usb_devices)


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org

More Python: https://pythonprogramminglanguage.com
