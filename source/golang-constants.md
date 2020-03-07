---
title: Golang golang-constants (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-constants'


## golang-constants

Golang beginners example: golang-constants

```go
package main

import "fmt"

func main() {
	//simple constants
	const stringConstant = "string"
	const boolConstant = true
	const intConstant = 1234

	fmt.Print(stringConstant)
	fmt.Print(boolConstant)
	fmt.Print(intConstant)

	//simple constant with type
	const float64Constant float64 = 1234.00

	fmt.Print(float64Constant)

	//multiple constants
	const color, code = "red", 255

	fmt.Print(color)
	fmt.Print(code)

	const (
		company string  = "Go Experts"
		salary  float64 = 50000.0
	)
	
	fmt.Print(company)
	fmt.Print(salary)
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
