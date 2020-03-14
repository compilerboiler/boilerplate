---
tags: ["go"]
date: 2020-02-14
title: go slice
---
In the <a href="https://golang.org">Go</a> programming language you can create <a href="https://golangr.com/arrays/">arrays</a>: collections.

You can create slices with the built-in **make()** function; you can create dynamically-sized arrays this way.

Remember that the usual array has a fixed size, that you would define in one of these two ways:

```go
var a [10]int
var a = []int64{ 1,2,3,4 }
```

What if you want an array that contains zeroes?

## Make() in Go

The make function allocates a zeroed array and returns a slice that refers to that array. The syntax of the make() function is:

    your_array := make([]type, length)

So if you'd have a program like this:

```go
package main

import "fmt"

func main() {
	a := make([]int, 5)
	printSlice("a", a)

}

func printSlice(s string, x []int) {
	fmt.Printf("%s len=%d cap=%d %v\n",
		s, len(x), cap(x), x)
}
```

It would output the array (contains a lot of zeros, the make() function does this):

    a len=5 cap=5 [0 0 0 0 0]

To change its size, change the second parameter

```go
a := make([]int, 50)
```


