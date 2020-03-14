---
date: 2020-02-16
title: file object in python
---
---
tags: ["python"]
date: 2020-02-16
title: file object in python
---
---
tags: ["python"]
date: 2020-02-14
title: file object in python
---
<a href="https://python.org">Python</a> supports file like objects, that don't write to the disk but stay in the memory.

You can create file like objects with <a href="https://docs.python.org/2/library/stringio.html">StringIO</a>. From Python version > 3 this is part of the <a href="https://docs.python.org/3/library/io.html">io module</a>. 

These files live only inside the computer memory, not on the disk. Python can <a href="https://pythonbasics.org/read-file/">read files</a> from the disk, but this article focuses on files in memory.

## StringIO

To start using file-like objects, first import the `io` module. Then create a new file with `io.StringIO()` where the parameter is the file contents.

```python
>>> import io
>>> 
>>> myFile = io.StringIO()
```

Now put some data into the file and read it with `.read()`

```python
>>> myFile = io.StringIO("Data into the file")
>>> myFile.read()
'Data into the file'
```

Try to read it again, the file is empty?

```python
>>> myFile.read()
''
```

No, the cursor is at the end. Set the cursor at position zero and you can read again.

```python
>>> myFile.seek(0)
0
>>> myFile.read()
'Data into the file'
>>> 
```

You can mimick file like behavior with it:

```python
>>> import io
>>> myFile = io.StringIO("Feeling good")
>>> data = myFile.read()
>>> print(data)
Feeling good
>>> 
```

## Write file

You can write data into the memory file too, by using the `.write()` method. This method is part of the object and as parameter takes a string (there's also regular <a href="https://pythonbasics.org/write-file/">write file</a>)

The `.write()` method lets you write any data into the file. The usual escape character work `\n` for a new line.
 
```python
>>> myFile = io.StringIO("")
>>> myFile.write("Write a line into the file\n")
>>> myFile.write("Second line.\n")
```

Then read the file with `.getvalue()`.

```python
>>> data = myFile.getvalue()
>>> data
'Write a line into the file\nSecond line.\n'
```

Close the memory file:

```python
>>> myFile.close()
>>> 
```

**Related links:**
* <a href="https://docs.python.org/3/library/io.html">Python io module, for working with streams</a>
* <a href="https://gumroad.com/l/dcsp">Learn Python, programming course</a>


