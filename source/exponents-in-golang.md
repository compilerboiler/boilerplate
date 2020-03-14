---
tags: ["go"]
date: 2020-02-14
title: exponents in golang
---
You can use exponents in <a href="https://golang.org/">Golang</a> *(Exponents are shorthand for repeated multiplication of the same thing by itself.)*. 

You need to import the math module to do that. It comes with the Pow function. This function works like this:

    math.Pow(base, exponent)

Go is not installed by default, so if you want to use Go, <a href="https://golangr.com/install/">install Go</a> first.

## Exponents example

Import the math module. Assign a base and exponent. Then you can call the Pow method and output the result:

```go
package main
import (
 "fmt"
 "math"
)

func main() {
 var exponent, base float64
 base = 2
 exponent = 3
 output := math.Pow(base, exponent)
 fmt.Printf("Result is %.2f\n", output)
}
```

## User input

For output, we wrote %.2f, which means two digits after the dot. You can use %f or %.4f if you need. What about input?

You can let the user type the base and exponent like this:

```go
package main
import (
 "fmt"
 "math"
)

func main() {
 var exponent, base float64
 fmt.Print("Base:")
 fmt.Scanln(&base)
 fmt.Print("Exponent:")
 fmt.Scanln(&exponent)
 output := math.Pow(base, exponent)
 fmt.Printf("Result is %.2f", output)
}
```

For numeric input you can use the Scanln() function, for plain text input you can use <a href="https://golangr.com/keyboard-input/">ReadString()</a>


