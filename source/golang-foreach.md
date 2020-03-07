---
title: Golang golang-foreach (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-foreach'


## golang-foreach

Golang beginners example: golang-foreach

```go
package main

import (
	"fmt"
)

// declare variables and define array content
var strarray = []string{"lorem", "ipsum", "dolor", "sit", "amet"}

func main() {
	for index, data := range strarray {
		fmt.Println(index, data)
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
