---
title: Golang golang-functionanonymous (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-functionanonymous'


## golang-functionanonymous

Golang beginners example: golang-functionanonymous

```go
package main

import (
	"fmt"
)

func main() {
	stop := make(chan bool)

	go func() {
		fmt.Println("this is Println inside an anonymous goroutine")
		stop <- true
	}()
	func() {
		fmt.Println("this is Println inside an anonymous function")
	}()
	<-stop
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
