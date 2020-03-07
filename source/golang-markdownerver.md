---
title: Golang golang-erver (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-erver'


## golang-erver

Golang beginners example: golang-erver

```go
package main

import (
	"net/http"
)

func main() {
	http.Handle("/", http.FileServer(http.Dir("./")))
	http.ListenAndServe(":8080", nil)
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
