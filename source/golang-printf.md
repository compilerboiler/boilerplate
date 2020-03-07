---
title: Golang golang-printf (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-printf'


## golang-printf

Golang beginners example: golang-printf

```go
package main

import "fmt"

type exampledata struct {
	a, b int
	c, d string
	e, f bool
	g, h float64
}

func printx(str string, data exampledata) {
	fmt.Printf("%"+str+":\t "+str+"\n", data)
}

func main() {
	x := exampledata{0, 1, "a", "b", true, false, 3.1415926535, 2.357111317192329}

	printx("%v", x)

	printx("%+v", x)

	printx("%#v", x)

	printx("%t", x)

	printx("%T", x)

	printx("%d", x)

	printx("%b", x)

	printx("%c", x)

	printx("%x", x)

	printx("%f", x)

	printx("%e", x)

	printx("%E", x)

	printx("%s", x)

	printx("%q", x)

	printx("%p", x)

	fmt.Println("\n\n", fmt.Sprintf("%+v", x))
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
