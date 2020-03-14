---
tags: ["python"]
date: 2020-02-16
title: format python dict as table
---
---
tags: ["python"]
date: 2020-02-14
title: format python dict as table
---
In <a href="https://python.org">Python</a> you can use formatted strings to output variables easily.  
Formatted string literals (f-strings) let you include variables inside a string by prefixing the string with f or F and writing expressions as {expression}.

If you have an f-string, you can use the `:10` to make sure it's 10 character wide. This let you create a nice table like this:

If you are new to Python, you should first <a href="https://pythonbasics.org">learn the basics</a>.

## Format dictionary as table with f-strings

If you have a newer version of Python (>3.5) you can use f-strings. These let you format strings nicely.

First we define a <a href="https://pythonbasics.org/dictionary/">dictionary</a>, then iterate over it with a for loop and format it with f-strings.

```python
>>> table = { "Alice": 12, "Jim": 15, "Tim": 19 }
>>> for name, id in table.items():
...     print(f'{name:10} => {id:10d}')
... 
Alice      =>         12
Jim        =>         15
Tim        =>         19
>>> 
```

If you want to add a header, just call the print function before. We removed  the decoration, making it easier to read.

```python
d = { "Alice": 128, "Bob": 256, "Tim": 512, "Jim": 1024 }
print(f"Key{' ':14} Value{' ':15}")
for k, v in d.items():
    print(f"{k:8}{v:15}")

```

This returns

```python
Key               Value               
Alice               128
Bob                 256
Tim                 512
Jim                1024
```

## Existing functions

You can also use an existing function, like this one I found on the web. Personally I prefer formatting with f-strings, but this may be what you are looking for.

```python
def printTable(myDict, colList=None):
    if not colList: 
        colList = list(myDict[0].keys() if myDict else [])
    myList = [colList] # 1st row = header
    for item in myDict: 
        myList.append([str(item[col] or '') for col in colList])
    #maximun size of the col for each element
    colSize = [max(map(len,col)) for col in zip(*myList)]
    #insert seperating line before every line, and extra one for ending. 
    for i in  range(0, len(myList)+1)[::-1]:
         myList.insert(i, ['-' * i for i in colSize])
    #two format for each content line and each seperating line
    formatStr = ' | '.join(["{{:<{}}}".format(i) for i in colSize])
    formatSep = '-+-'.join(["{{:<{}}}".format(i) for i in colSize])
    for item in myList: 
        if item[0][0] == '-':
            print(formatSep.format(*item))
        else:
            print(formatStr.format(*item))

d = { "Alice": 128, "Bob": 256, "Tim": 512, "Jim": 1024 }
printTable([d])
```

This outputs:


```
------+-----+-----+-----
Alice | Bob | Tim | Jim 
------+-----+-----+-----
128   | 256 | 512 | 1024
------+-----+-----+-----
```

**Related links:**
* <a href="https://gumroad.com/l/dcsp">Python programming course</a>
* <a href="https://www.python.org/dev/peps/pep-0498/">Python formatted strings, f-strings</a>
