---
title: Golang golang-sortingInGo (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-sortingInGo'


## golang-sortingInGo

Golang beginners example: golang-sortingInGo

```go
package main

import "fmt"
import "sort"

func main() {
	strs := []string{"c", "a", "b"}
	sort.Strings(strs)
	fmt.Println("Strings:", strs)

	ints := []int{7, 2, 4}
	sort.Ints(ints)
	fmt.Println("Ints:   ", ints)

	s := sort.IntsAreSorted(ints)
	fmt.Println("Sorted: ", s)
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
