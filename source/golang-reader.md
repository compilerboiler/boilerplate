---
title: Golang golang-reader (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-reader'


## golang-reader

Golang beginners example: golang-reader

```go
package main

import (
	"./packages/"
	"bufio"
	"log"
)

func main() {
	M := foobar.NewReader()

	bytes := make([]byte, 255)

	bufio.NewReader(M).Read(bytes)

	log.Printf("%s", bytes)
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
