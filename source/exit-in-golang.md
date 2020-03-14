---
tags: ["go"]
date: 2020-02-14
title: exit in golang
---
<a href="https://golang.org/">Go</a> is a popular programming language, that at first glance seems a bit like C/Java. The famous hello world program looks like this:

```go
package main
import "fmt"

func main() {
	fmt.Println("Hello, World")
}
```

You may wonder, where is *return* or *exit*? How does exit work in Golang?

## Exit program

If you want to quit your golang program, you can use os.Exit. This is part of the os module.

From the <a href="https://golang.org/pkg/os/#Exit">golang docs</a>:

*"Exit causes the current program to exit with the given status code. Conventionally, code zero indicates success, non-zero an error. The program terminates immediately; deferred functions are not run."*

## Example

*os.Exit* exits the program immediately with a given status. 

```go
package main
import (
 "os"
)

func main() {
  os.Exit(4)
}
```

Shown below the output:

    > go run test.go
    exit status 4

The status is shown in the terminal like this. *os.Exit()* can be used to exit the program normally without an error like this:

```go
package main
import (  
 "os"
)
    
func main() {
  os.Exit(0)
}
```

This returns to the terminal without showing anything.

**Related links:**
* <a href="https://golang.org/">Go Programming Language</a>
* <a href="https://golangr.com/">Golang tutorial</a>

