---
title: Golang golang-log (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-log'


## golang-log

Golang beginners example: golang-log

```go
package main

import (
	"log"
)

func main() {
	log.SetFlags(log.Ltime | log.Lshortfile)

	log.Println("first log output")
	log.Printf("second log output\n")
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
