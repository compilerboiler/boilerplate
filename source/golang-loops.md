---
tags: ["go"]
date: 2020-02-14
title: golang loops
---
A loop lets you repeat code. There are different types of loops, one of them is a for loop. For loops in <a href="https://golang.org/">Go (golang)</a> are more similar to C/Java than Python. In Python the syntax is

    for i in range(1,10):

In C/Java the syntax is

    for (i = 1; i <= 10; i++) {

But in Golang

    for i := 1; i <= 10; i++ {

So it's inspired by those languages. 

## For loop explained

In the above program, what does it mean?
First the initial value of variable i is 1.

    i := 1;

The conditional statement will checks if i <= 10.

    i <= 10;

If that is true it stops the loop. If not, it continues inside the loop.
The post statement adds 1 to i every iteration.

    i++

In other words, i++ is the same as i = i + 1

## Example

A program with a for loop counting from 1 to 10 becomes:

```go
package main

import (  
    "fmt"
)

func main() {  
    for i := 1; i <= 10; i++ {
        fmt.Printf(" %d",i)
    }
}
```

The other stuff is loading go, importing the fmt module and the main loop.
You can also use <a href="https://golangr.com/while/">while loops in golang</a>

**Related links:**
* <a href="https://golang.org/">Golang official website</a> 
* <a href="https://golangr.com/">Go tutorial</a>


