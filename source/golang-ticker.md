---
title: Golang golang-ticker (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-ticker'


## golang-ticker

Golang beginners example: golang-ticker

```go
package main

import (
	"crypto/rand"
	"fmt"
	"time"
)

func getrandom() int {
	b := make([]byte, 2)
	rand.Read(b)
	number := uint32(b[0]) | (uint32(b[1]) << 8)
	return int(number)
}

func main() {
	var x int
	ticker := time.NewTicker(time.Millisecond * 500)
	go func() {
		for t := range ticker.C {
			fmt.Printf("ticker:\t%d\tat:\t", x)
			fmt.Println(t)
		}
	}()

	go func() {
		for {
			x = getrandom()
		}
	}()

	time.Sleep(time.Second * 10)
	ticker.Stop()
	fmt.Println("Ticker stopped")
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
