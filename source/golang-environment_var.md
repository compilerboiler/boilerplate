---
title: Golang golang-environment var (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-environment var'


## golang-environment var

Golang beginners example: golang-environment var

```go
package main

import (
	"fmt"
	"os"
	"strings"
)

func main() {
	os.Setenv("FOO", "1")
	fmt.Println("FOO:", os.Getenv("FOO"))
	fmt.Println("BAR:", os.Getenv("BAR"))

	fmt.Println()
	for _, e := range os.Environ() {
		pair := strings.Split(e, "=")
		fmt.Println(pair[0])
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
