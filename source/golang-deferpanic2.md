---
title: Golang golang-deferpanic2 (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-deferpanic2'


## golang-deferpanic2

Golang beginners example: golang-deferpanic2

```go
package main

import (
	"fmt"
)

func main() {
	stop := 10
	for i := 0; i < 15; i++ {
		func() {
			defer func() {
				recover()
			}()

			if i == 10 {
				fmt.Println("i10")
				panic(0)
			}
			if i == 14 {
				fmt.Println("i14")
				i = 0
				stop--
				panic(0)
			}
		}()
		if stop == 0 {
			break
		}
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
