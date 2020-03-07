---
title: Golang golang-map01 (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-map01'


## golang-map01

Golang beginners example: golang-map01

```go
package main

import "fmt"

func main() {

    m := make(map[string]int)

    m["a"] = 1
    m["b"] = 2

    a := m["a"]
    fmt.Println("a: ", a)

    delete(m, "b")
    b, ok := m["b"]
    fmt.Println("b: ", b)
    fmt.Println("ok? ", ok)
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
