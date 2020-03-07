---
title: Golang golang-deleteFromSlice (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-deleteFromSlice'


## golang-deleteFromSlice

Golang beginners example: golang-deleteFromSlice

```go
package main

import "fmt"

func main() {
	mySlice := []int{1, 2, 3, 4, 5, 6, 7, 8, 9}

	// Deleting from a slice is basically appending the entire slice to itself, but excluding the deleted item
	mySlice = append(mySlice[:4], mySlice[5:]...)
	fmt.Println(mySlice)
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
