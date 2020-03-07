---
title: Golang golang-cat (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-cat'


## golang-cat

Golang beginners example: golang-cat

```go
package main

import (
	"bytes"
	"fmt"
	"strconv"
)

func main() {
	var buffer bytes.Buffer
	for i := 0; i < 32; i++ {
		buffer.WriteString("a")
	}
	s := buffer.String()
	for i := 0; i < 8192; i++ {
		s += strconv.Itoa(i)
	}
	s += buffer.String()
	for i := 0; i < 512; i++ {
		s = "pre" + s
	}
	fmt.Println(s)
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
