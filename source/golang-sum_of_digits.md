---
title: Golang golang-sum of digits (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-sum of digits'


## golang-sum of digits

Golang beginners example: golang-sum of digits

```go
package main

import (
	"bufio"
	"fmt"
	"os"
	"strconv"
	"strings"
)

func main() {
	fmt.Print("Enter digits to sum separated by a space:")
	str, err := getline()
	if err == nil {
		fmt.Println("Here is the result:", sumNumbers(str))
	}
}

func getline() (string, error) {
	return bufio.NewReader(os.Stdin).ReadString('\n')
}

func sumNumbers(str string) float64 {
	var sum float64
	for _, v := range strings.Fields(str) {
		i, err := strconv.ParseFloat(v, 64)
		if err != nil {
			fmt.Println(err)
		} else {
			sum += i
		}
	}
	return sum
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
