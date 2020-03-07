---
title: Golang golang-functionclosure (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-functionclosure'


## golang-functionclosure

Golang beginners example: golang-functionclosure

```go
package main

import (
	"fmt"
	"time"
)

func initTimeSeq() func() int {
	t := time.Now().UnixNano()
	return func() int {
		return int(time.Now().UnixNano() - t)
	}
}

func main() {
	timeSince := initTimeSeq()

	fmt.Println(timeSince())

	fmt.Println(timeSince())

	time.Sleep(1 * time.Second)

	fmt.Println(timeSince())

	time.Sleep(120 * time.Millisecond)

	fmt.Println(timeSince())

	timeSince = initTimeSeq()

	time.Sleep(1300 * time.Millisecond)

	fmt.Println(timeSince())

	fmt.Println(timeSince())

	fmt.Println(timeSince())
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
