---
title: writingFiles (snippet)
date: 2019-02-07
tags: ["python"]
---
Python example 'writingFiles'


## writingFiles

Python beginners example: writingFiles

```python
# Writing files

# Enter file name which is in same directory as that of the program
fileName = str(input('File name : ')) 
fileToWrite = open(fileName, 'w') # 'w' writes to the file
textToWrite = str(input('Text to write : '))
fileToWrite.write(textToWrite) # writing file
fileToWrite.close() # closing the file


```

## Useful links

- Learn Python: https://pythonbasics.org
- Download Python: https://python.org
- Another Python site: https://pythonprogramminglanguage.com
