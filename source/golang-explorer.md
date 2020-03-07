---
title: Golang golang-explorer (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-explorer'


## golang-explorer

Golang beginners example: golang-explorer

```go
package main

import (
	"fmt"
	"io/ioutil"
	"os"
)

func main() {
	wd, err := os.Getwd()
	if err == nil {
		fmt.Println(wd)
		files, _ := ioutil.ReadDir(wd)
		for _, f := range files {
			fmt.Printf("-> %v\n", f.Name())
		}
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
