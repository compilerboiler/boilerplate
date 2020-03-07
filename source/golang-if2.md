---
title: Golang golang-if2 (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-if2'


## golang-if2

Golang beginners example: golang-if2

```go
package main

import (
	"fmt"
)

func f1(b bool) bool {
	fmt.Printf("f1: %v\n", b)
	return b
}

func f2(b bool) bool {
	fmt.Printf("f2: %v\n", b)
	return b
}

func f3(b bool) bool {
	fmt.Printf("f3: %v\n", b)
	return b
}

func main() {
	if f1(true) == true {
		fmt.Println("✔")
	}

	if f1(true) {
		fmt.Println("✔")
	}

	fmt.Println("\nAND")
	if f1(true) && f2(true) {
		fmt.Println("✔")
	}

	fmt.Println("\nAND")
	if f1(false) && f2(true) {
		fmt.Println("✔")
	}

	fmt.Println("\nAND")
	if f1(true) && f2(false) && f3(true) {
		fmt.Println("✔")
	}

	fmt.Println("\nOR")
	if f1(true) || f2(true) {
		fmt.Println("✔")
	}

	fmt.Println("\nOR")
	if f1(true) || f2(true) {
		fmt.Println("✔")
	}

	fmt.Println("\nAND+OR")
	if f1(true) && f2(false) || f3(true) {
		fmt.Println("✔")
	}

	fmt.Println("\n(AND)+OR")
	if (f1(true) && f2(false)) || f3(true) {
		fmt.Println("✔")
	}

	fmt.Println("\n(AND)+OR")
	if (f1(true) && f2(true)) || f3(false) {
		fmt.Println("✔")
	}

	fmt.Println("\nAND+(OR)")
	if f1(true) && (f2(false) || f3(true)) {
		fmt.Println("✔")
	}

	fmt.Println("\nAND+(OR)")
	if f1(true) && (f2(true) || f3(false)) {
		fmt.Println("✔")
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
