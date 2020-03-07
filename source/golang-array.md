---
title: Golang golang-array (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-array'


## golang-array

Golang beginners example: golang-array

```go
package main

// import required modules
import (
	"fmt"
)

// declare variables and define array content
var strarray = []string{"lorem", "ipsum", "dolor", "sit", "amet"}
var intarray = []int{1, 2, 4, 8, 16}
var mapone = map[int]string{}
var maptwo = map[string]interface{}{}

func main() {

	// do this five times
	for i := 0; i != 5; i++ {

		// print the $th value of the intarray and the strarray
		fmt.Println(intarray[i], "\t", strarray[i])

		mapone[intarray[i]] = strarray[i]
		maptwo[strarray[i]] = mapone
	}
	fmt.Println(mapone)
	fmt.Println(maptwo)
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
