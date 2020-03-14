In <a href="https://golang.org/">Golang</a> methods can take <a href="https://golangr.com/struct/">structs</a> as parameter. You may be familiar with this from other languages, where you post objects as <a href="https://golangr.com/methods/">method</a> parameter.

This is great, because while Go doesn't support object orientated programming in the traditional sense, this gives you the feel of objects.

## Structs as method parameter

In this article we'll do an example where a method takes a struct as parameter. First we define a struct

```go
type Student struct {
    name     string
    year     int
}
```

Then create a new struct "instance"

```go
s1 := Student { name: "Sam", year:   1, }
```

Then you can call a method on the struct:

```go
s1.displayYear()
```

So we have the golang code for this example below:

```go
package main

import (
    "fmt"
)

type Student struct {
    name     string
    year     int
}

func (s Student) displayYear() {
    fmt.Printf("Student year of %s is %d\n", s.name, s.year)
}

func main() {
    s1 := Student { name: "Sam", year:   1, }
    s1.displayYear()
}
```

That outputs the data we passed as parameter

    ➜  go run example.go
    Year of Sam is 1

You can create all kinds of structs to work with in your code:

```go
    s1 := Student { name: "Sam", year:   1, }
    s2 := Student { name: "Amy", year:   5, }
    s3 := Student { name: "May", year:   3, }
    s4 := Student { name: "Yas", year:   4, }
```

On all of these you can call the same method

```go
    s2.displayYear()
    s3.displayYear()
    s4.displayYear()
```
