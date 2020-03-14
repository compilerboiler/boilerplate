In <a href="https://golang.org">Go</a> you can easily slice <a href="https://golangr.com/strings/">strings</a> or <a href="https://medium.com/rungo/the-anatomy-of-arrays-in-go-24429e4491b7">arrays</a>. As the name implies, a slice is a subset of the whole.

This is unlike C where you would have to use strcpy or other tricks to slice a string. (this is a lot of work)

Not so in Golang, to take a slice is much easier.

## String slice in Go

You can slice a string simply by using brackets and start and end index, as if you were using Python.

The format to slice is:

```go
a[low : high]
```

So to slice from 1 to 3, you would use

```go
a[1:4]
```

A string slice example is shown below. First a string (st) is defined. Then it's sliced and given as input to the Println function:

```go
package main

import "fmt"

func main() {
	st := "Hello World"
	fmt.Println(st[1:3])
}
```

If you run the program it will output a slice of the string st:

```go
el

Program exited.
```

To grab the first word, use st[0:5]. You can do this for arrays too!

```go
package main

import "fmt"

func main() {
	primes := [6]int{2, 3, 5, 7, 11, 13}

	var s []int = primes[1:4]
	fmt.Println(s)
}
```

Here we define an array of primes and then take a slice out of that. That slice is stored as a new variable and shown to the screen.


