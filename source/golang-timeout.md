---
title: Golang golang-timeout (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-timeout'


## golang-timeout

Golang beginners example: golang-timeout

```go
package main

import (
	"crypto/rand"
	"fmt"
	"time"
)

func getrandom() int {
	b := make([]byte, 3)
	rand.Read(b)
	number := uint32(b[0]) | (uint32(b[1]) << 8) | (uint32(b[2]) << 16)
	return int(number)
}

func randomcalculate(i int) int {
	var r, x int
	for a := 0; a < 1000; a++ {
		r = getrandom() / 1337
		x = (i + r) / 42
		fmt.Printf("%d\t+\t%d\t=\t%d\n", i, r, x)
		i = x
		time.Sleep(15 * time.Millisecond)
	}
	return i
}

func main() {
	chanx := make(chan int)
	go func() {
		chanx <- randomcalculate(6)
	}()
	select {
	case res := <-chanx:
		fmt.Println(res)
	case <-time.After(time.Millisecond * 150):
		fmt.Println("timeout")
	}

}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
