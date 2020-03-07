---
title: Golang golang-pointer (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-pointer'


## golang-pointer

Golang beginners example: golang-pointer

```go
package main

import (
	"fmt"
)

func plusOne(in *int) {
	*in++
}

func main() {
	var value int
	value = 5

	fmt.Printf("value: %v\n", value)
	plusOne(&value)
	fmt.Printf("value: %v\n", value)
	plusOne(&value)
	plusOne(&value)
	plusOne(&value)
	fmt.Printf("value: %v\n", value)
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
