---
title: Golang golang-return (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-return'


## golang-return

Golang beginners example: golang-return

```go
package main

// import required modules
import (
	"fmt"
)

func named() (str string) {
	str = "lorem"
	return
}

func typed() string {
	var str = "ipsum"
	return str
}

// main function
func main() {
	fmt.Println(named())
	fmt.Println(typed())
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
