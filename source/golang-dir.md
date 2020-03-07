---
title: Golang golang-dir (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-dir'


## golang-dir

Golang beginners example: golang-dir

```go
package main

import (
	"fmt"
	"os"
	"strings"
)

func main() {
	dir, _ := os.Getwd()
	fmt.Println(strings.Replace(dir, " ", "\\ ", -1))
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
