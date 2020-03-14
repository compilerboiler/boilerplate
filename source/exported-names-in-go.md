---
tags: ["go"]
date: 2020-02-14
title: exported names in go
---
Many packages have variables (constants). In the <a href="https://golangr.com/">Go</a> programming language, exported <a href="https://golangr.com/variables/">variable</a> names are a bit different.

Before playing around with Go packages and constants, you should be able to <a href="https://golangr.com/hello-world/">run go programs</a>

## Example

For example, if you import the math module you can access some of its variables:

```go
fmt.Println(math.Pi)
fmt.Println(math.E)
```

These variables reside in the math module. When importing a package, you can refer only to its exported names.

Lets try that in a program

```go
package main

import (
	"fmt"
	"math"
)

func main() {
	fmt.Println(math.Pi)
	fmt.Println(math.E)
	fmt.Println(math.Phi)
	fmt.Println(math.SqrtE)
}
```

*If a variable does not start with a capital letter, it is not exported.*

So if you'd try

```go
fmt.Println(math.e)
```

That wouldn't work, because only variables with a capital letter are exported.

## Constants

So how do you know which variables exist in a module?

One way to find out is in the <a href="https://golang.org/pkg/math/">golang package docs</a>. Open the name of the package and search for constants.

You can browse some of the main packages <a href="https://golang.org/pkg/">here</a>


