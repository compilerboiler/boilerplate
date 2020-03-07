---
title: Golang golang-regex (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-regex'


## golang-regex

Golang beginners example: golang-regex

```go
package main

import (
	"fmt"
	"regexp"
)

var variable string
var strarray []string
var r = regexp.MustCompile("[^\\s]+")

func main() {
	variable = "Lorem  Ipsum  Dolor   Sit  Amet"
	strarray = r.FindAllString(variable, -1)
	for i := 0; i < len(strarray); i++ {
		fmt.Println(strarray[i])
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
