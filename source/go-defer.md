---
tags: ["go"]
date: 2020-02-16
title: go defer
---
---
tags: ["go"]
date: 2020-02-14
title: go defer
---
In the <a href="https://golang.org">Golang</a> programming language you can use the defer statement. A defer statement defers the execution of a function until the surrounding <a href="https://golangr.com/methods/">function</a> returns. 

So in practice, that means first finish the current function before executing the deferred function.

## Examples 

The program below is a go program that imports the "fmt" module for output and then calls the Println function twice. It uses the defer statement;

```go
package main

import "fmt"

func main() {
	defer fmt.Println("world")
	fmt.Println("hello")
}
```

The deferred call's arguments are evaluated immediately, but the function call is not executed until the surrounding function returns.

Instead of the output "hello world", it outputs:

```
hello
world

Program exited.
```

The Println function "world" is only called once the function main is finished.

## Defer

If you would extend the function with several calls, it will output world last. The program remains in normal execution order.

```go
package main

import "fmt"

func main() {
	defer fmt.Println("world")
	fmt.Println("hello")
	fmt.Println("there")
	fmt.Println("the")
}
```

You can defer more than one function call, then all the deferred functions are executed after the main cycle has completed:

```go
defer fmt.Println("world")
defer fmt.Println("hello")
defer fmt.Println("there")
fmt.Println("the")
```

**Related links:**
* <a href="https://golangr.com/defer/">Defer statement</a>
* <a href="https://golangr.com/">Learn Go</a>
