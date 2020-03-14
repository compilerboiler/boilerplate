---
tags: ["go"]
date: 2020-02-14
title: function values in go
---
In the <a href="https://golang.org/">Go</a> programming language, <a href="https://golangr.com/methods/">functions</a> are values. That means that you can pass a function as parameter in a function.

For example, you can define a function `mul` which multiplies x and y. Then it returns the result.

```go
mul := func(x, y float64) float64 {
    return x*y
}
```

Then you could assign the output to a variable and output it

```go
var a float64
a = mul(3,5)
fmt.Println(a)
```

However, you can directly output it as a result to the print function

```go
fmt.Println(mul(5, 12))
```

The program would then be:

```go
package main

import (
	"fmt"
)

func main() {
	mul := func(x, y float64) float64 {
		return x*y
	}
	fmt.Println(mul(5, 12))
}
```

This results in:

    60
    
    Program exited.

**Related links:**
* <a href="https://golang.org/">Go website</a>
* <a href="https://golangr.com/">Learn Go</a>

