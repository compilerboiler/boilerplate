---
tags: ["go"]
date: 2020-02-14
title: go classes
---
<a href="https://golang.org">Go</a> is not a pure object oriented programming language. In truth, Go does not provide classes. Go uses <a href="https://golangr.com/struct/">structs</a> instead. 

Create a file example.go with the struct student. You can create a new person using this struct as the example shows:

```go
package main

import "fmt"

type student struct {
    FirstName       string
    LastName        string
}

func main() {
    s1 := student{ FirstName: "Nils", LastName: "Bohr" }
    fmt.Println(s1.FirstName)
}
```

This program outputs in:

```
➜  go run app.go   
Nils
```

You can create multiple students like this:

```go
s1 := student{ FirstName: "Nils", LastName: "Bohr" }
s2 := student{ FirstName: "Albert", LastName: "Einstein" }
fmt.Println(s1.FirstName)
fmt.Println(s2.FirstName)
```

## Methods

So what about methods? Methods can be "added to structs". You can create a method that takes a struct as parameter, like this:

```go
func (s student) name() {
    fmt.Printf("%s %s\n", s.FirstName, s.LastName)
}
```

Then you can call it like this:

```go
s1.name()
s2.name()
```

That makes the program:

```go
package main

import "fmt"

type student struct {
    FirstName       string
    LastName        string
}

func (s student) name() {
    fmt.Printf("%s %s\n", s.FirstName, s.LastName)
}

func main() {
    s1 := student{ FirstName: "Nils", LastName: "Bohr" }
    s2 := student{ FirstName: "Albert", LastName: "Einstein" }
    s1.name()
    s2.name()
}
```

**Related links:**
* <a href="https://golang.org">Go programming language</a>
* <a href="https://golangr.com/">Learn Go</a>
