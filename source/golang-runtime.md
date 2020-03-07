---
title: Golang golang-runtime (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-runtime'


## golang-runtime

Golang beginners example: golang-runtime

```go
package main

import (
	"fmt"
	"log"
	"runtime"
	"time"
)

func Debug(format string, a ...interface{}) {
	_, file, line, _ := runtime.Caller(1)
	info := fmt.Sprintf(format, a...)

	log.Printf("%s:%d %v", file, line, info)
}

func foobar(format string, a ...interface{}) {
	Debug(format, a)
}

func main() {
	foobar("test: %v\n", time.Now())
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
