---
title: Golang golang-functionmain (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-functionmain'


## golang-functionmain

Golang beginners example: golang-functionmain

```go
package main

import (
	"fmt"
)

var i int

func init() {
	fmt.Println("the init function gets started at first")
}

func main() {
RESTART:
	fmt.Println("the main function gets called immediately after")
	if i < 3 {
		i++
		fmt.Println("we can also call the main function ourself (but not init)")
		goto RESTART
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
