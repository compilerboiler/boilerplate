---
title: Golang golang-ackermann (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-ackermann'


## golang-ackermann

Golang beginners example: golang-ackermann

```go
package main

import (
	"fmt"
	"os"
	"strconv"
)

func ack(n, m int64) int64 {
	for n != 0 {
		if m == 0 {
			m = 1
		} else {
			m = ack(n, m-1)
		}
		n = n - 1
	}
	return m + 1
}

func main() {
	if len(os.Args) > 2 {
		ia1, _ := strconv.ParseInt(os.Args[1], 10, 0)
		ia2, _ := strconv.ParseInt(os.Args[2], 10, 0)
		fmt.Println(ack(ia1, ia2))
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
