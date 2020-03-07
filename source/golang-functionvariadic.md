---
title: Golang golang-functionvariadic (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-functionvariadic'


## golang-functionvariadic

Golang beginners example: golang-functionvariadic

```go
package main

import "fmt"

func sum(numbers ...int) int {
	var total int = 0
	for _, number := range numbers {
		total += number
	}
	return total
}

func main() {
	fmt.Println(sum(2, 3, 5, 7, 11, 13, 17, 19, 23, 29))

	numbers := []int{31, 37, 41, 43, 47, 53, 59}

	fmt.Println(sum(numbers...))
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
