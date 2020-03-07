---
title: Golang golang-label (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-label'


## golang-label

Golang beginners example: golang-label

```go
package main

import (
	"fmt"
)

func BreakExample() {
	fmt.Println("\n\nBreak Example")
	for i := 0; i < 10; i++ {
		fmt.Print("\ni:", i)
		if i > 5 {
			break
		}
		fmt.Print(".")
	}
}

func ContinueExample() {
	fmt.Println("\n\nContinue Example")
	for i := 0; i < 10; i++ {
		fmt.Print("\ni:", i)
		if i > 5 {
			continue
		}
		fmt.Print(".")
	}
}

func ContinueToLabelExample() {
	var i, j int
	fmt.Println("\n\nContinue to Label Example")
OUT:
	for i = 0; i < 10; i++ {
		for j = 0; j < 10; j++ {
			fmt.Print("\ni:", i, "j:", j)
			if i > 2 && j > 2 {
				continue OUT
			}
			fmt.Print(".")
		}
	}

	fmt.Println("i:", i, "j:", j)
}

func GotoExample() {
	fmt.Println("\n\nGoto Example")
	var i = 0

START:
	i++
	fmt.Println("i:", i)
	if i < 10 {
		goto START
	}

	fmt.Println("finish")
}

func GotoExample2() {
	fmt.Println("\n\nGoto Example 2")
	var i = 0

START:
	i++
	fmt.Println("i:", i)
	if i < 10 {
		goto START
	} else {
		goto END
	}

	fmt.Println("never print this!!!")

END:
}

func main() {
	BreakExample()
	ContinueExample()
	ContinueToLabelExample()
	GotoExample()
	GotoExample2()
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
