---
title: geoMean (snippet)
date: 2019-02-07
tags: ["python"]
---

## geoMean

Python beginners example: geoMean

```python
# Add path, encoding

import math


# Geometric Mean:
# Calculates the geometric mean of 
# two numbers 
# formula: f(x, y) = square_root(x*y)

geoMean = lambda x, y: math.sqrt(x*y)


while True:
	if input("Start [Y/n]?  ").strip().lower() == "y":
		print(" [Res] = " + str(geoMean(float(input("\nX? ")), float(input("Y? ")))) + "\n\n")
	else:
		print("\n\nGoodBye!")
		break


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
