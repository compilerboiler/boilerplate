---
title: healthScore (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'healthScore'

Functions in program: 
* `def healthScore():`

## healthScore

Python beginners example: healthScore

```python
# Health Calculator

# func to show health score of user
def healthScore():
	print(' ')
	numberOfFruits = int(input('Number Of Fruits You Eat in Week : ')) 
	numberOftimesFastFood = int(input('Number of Times You Eat FastFood in a Week : '))  
	cigars = int(input('Cigars You Smoke In A Week : ')) 
	workoutTime = int(input('How Much minutes You Workout EveryDay : '))  
	bodyMassIndex = int(input('Whats Your BodyMassIndex(BMI) : '))
	if 18 < bodyMassIndex < 26 :
		print(' ')
		healthScore = (numberOfFruits + workoutTime + bodyMassIndex ) - (cigars + numberOftimesFastFood) 
		print(healthScore)
	else :
		print(' ')
		healthScore = (numberOfFruits + workoutTime) - (cigars + numberOftimesFastFood + bodyMassIndex )
		print(healthScore)	

# main code
while True:
	startOrEnd = str(input('Start or End : '))
	if startOrEnd == 'Start':
		print(healthScore())
		continue
	else :
		quit()	


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
