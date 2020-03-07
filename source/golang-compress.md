---
title: Golang golang-compress (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-compress'


## golang-compress

Golang beginners example: golang-compress

```go
package main

import (
	"compress/gzip"
	"flag"
	"io"
	"os"
)

var n = flag.Int("n", 6, "Compression level (0-9)")

func main() {
	flag.Parse()
	c, _ := gzip.NewWriterLevel(os.Stdout, *n)

	io.Copy(c, os.Stdin)
	c.Close()
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
