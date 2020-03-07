---
title: Golang golang-shell (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-shell'


## golang-shell

Golang beginners example: golang-shell

```go
package main

import (
	"fmt"
	"os"
	"os/exec"
)

func main() {
	out, err := exec.Command("echo", "Hello", "world").Output()
	if err != nil {
		fmt.Printf("%s", err)
		os.Exit(1)
	} else {
		fmt.Printf("%s\n", out)
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
