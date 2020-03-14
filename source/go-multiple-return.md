---
tags: ["go"]
date: 2020-02-14
title: go multiple return
---
Typically a function only returns one variable, but why should that be?

In the <a href="https://golang.org/">Go</a> programming language, <a href="https://golangr.com/methods/">functions</a> can return multiple values. This is unlike C, where a function only returns one value. However there are other languages that support multiple return, like Python.

On syntax we can say, the type of return value is written at the end instead of in the beginning. Where in C you would have

```c
int plus(int a, int b) {
```

In Go the same function would be

```go
func plus(a,b int) (int) {
```

## Multiple return

As I mentioned above, functions in Go can return multiple values.
You can have a function like this:

```go
func swap(x, y string) (string, string) {
	return y, x
}
```

This function then returns two variables of the type <a href="https://golangr.com/strings/">string</a>, but it also takes two parameters of the type string.

You can store the output like this:


```go
a, b := swap("hello", "world")
```

So if you put that in a program, you would have this:

```go
package main

import "fmt"

func swap(x, y string) (string, string) {
	return y, x
}

func main() {
	a, b := swap("hello", "world")
	fmt.Println(a, b)
}
```

That gives you new options when programming. You could have a multiply function that returns the input values and the output.

```go
package main

import "fmt"

func multiply(a,b int) (int,int,int) {
    return a,b,a*b
}

func main() {
    a, b, c := multiply(16,13)
    fmt.Println(a,b,c)
}
```

If you run it you'll see that:

```
➜  ~ go run example.go
16 13 208
```
