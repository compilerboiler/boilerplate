---
title: Golang golang-interfaces (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-interfaces'


## golang-interfaces

Golang beginners example: golang-interfaces

```go
package main

import "fmt"

func FuncWithInterface(emptyinterface interface{}) {
	switch t := emptyinterface.(type) {
	case string:
		fmt.Print("type: string\t")
	case int:
		fmt.Print("type: int\t")
	case bool:
		fmt.Print("type: bool\t")
	default:
		fmt.Printf("type: %v\t", t)
	}

	fmt.Printf("data: %#v\n", emptyinterface)
}

func main() {
	var emptyinterface = [3]interface{}{}

	emptyinterface[0] = 23
	emptyinterface[1] = "foobar"
	emptyinterface[2] = false

	fmt.Printf("data: %v\n", emptyinterface)

	for _, v := range emptyinterface {
		FuncWithInterface(v)
	}

}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
