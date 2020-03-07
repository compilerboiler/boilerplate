---
title: Golang golang-input (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-input'


## golang-input

Golang beginners example: golang-input

```go
package main

import (
	"bufio"
	"fmt"
	"os"
)

func main() {
	//arguments
	if 1 < len(os.Args) {
		fmt.Print(len(os.Args) - 1)
		fmt.Println(" arguments provided")
	}
	/*
		//Scanf to wait for an input
		fmt.Println("Enter a number")
		var i int
		_, err := fmt.Scanf("%d", &i)
		if err != nil {
			fmt.Println("not a number")
		} else {
			fmt.Print(i)
			fmt.Println(" is a number")
		}
	*/
	//Stdin read buffer
	fmt.Println("Enter a string")
	bio := bufio.NewReader(os.Stdin)
	line, _, err := bio.ReadLine()
	if err != nil {
		fmt.Println(err)
	} else {
		//fmt.Println("you entered \"" + string(line) + "\"")
		for _, char := range string(line) {
			fmt.Println(char)
		}
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
