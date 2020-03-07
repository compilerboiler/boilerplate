---
title: Golang golang-wait (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-wait'


## golang-wait

Golang beginners example: golang-wait

```go
package main

import (
	"fmt"
	"sync"
	"time"
)

func f(w *sync.WaitGroup, sec int) {
	fmt.Println("a")
	time.Sleep(time.Duration(sec) * time.Second)
	fmt.Println("b")
	w.Done()
}

func main() {
	fmt.Println("start")
	var w sync.WaitGroup
	w.Add(2)

	go func(w *sync.WaitGroup, sec int) {
		fmt.Println("c")
		<-time.After(time.Duration(sec) * time.Millisecond)
		fmt.Println("d")
		w.Done()
	}(&w, 2500)

	go f(&w, 4)

	w.Wait()

	time.Sleep(900000000 * time.Nanosecond)

	fmt.Println("finish")
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
