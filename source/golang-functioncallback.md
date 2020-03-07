---
title: Golang golang-functioncallback (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-functioncallback'


## golang-functioncallback

Golang beginners example: golang-functioncallback

```go
package main

import "fmt"

func timestwo(f func(int) int, x int) int {
	return f(x * 2)
}

func main() {
	fmt.Printf("%v\n", timestwo(func(i int) int {
		return i * 2
	}, 32))
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
