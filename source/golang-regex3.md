---
title: Golang golang-regex3 (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-regex3'


## golang-regex3

Golang beginners example: golang-regex3

```go
package main

import (
	"fmt"
	"simonwaldherr.de/go/golibs/regex"
)

func main() {
	fmt.Println(regex.ReplaceAllString("FooBaR LoReM IpSuM", "\\W", ""))
	fmt.Println(regex.ReplaceAllString("FooBaR LoReM IpSuM", "[a-z]", ""))
	fmt.Println(regex.ReplaceAllString("FooBaR LoReM IpSuM", "[A-Z]", ""))
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
