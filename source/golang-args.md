---
title: Golang golang-args (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-args'


## golang-args

Golang beginners example: golang-args

```go
package main

// import required modules
import (
	"fmt"
	"os"
)

// main function
func main() {

	// print each argument
	for i := 1; i < len(os.Args); i++ {
		fmt.Println(os.Args[i])
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
