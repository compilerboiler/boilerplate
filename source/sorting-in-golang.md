---
tags: ["go"]
date: 2020-02-16
title: sorting in golang
---
---
tags: ["go"]
date: 2020-02-14
title: sorting in golang
---
Sorting numbers in <a href="https://golang.org/">Golang</a> is nothing like C. If you don't know about the C language, it makes you write a sorting function yourself. It is much easier in Go. There's a package named sort.

This package has several methods to sort:

* sort.Ints
* sort.Float64s
* sort.Strings

Use the method you need for the datatype. 

Before trying this, make sure you can <a href="https://golangr.com/hello-world/">run Go programs</a>.

## Sort ints

This example shows you how to use the sort method for integers. Values are sorted from low to high.

```go
package main

import (
        "fmt"
        "sort"
)

func main() {
        s := []int{5, 6, 3, 2, 1, 4} // unsorted
        sort.Ints(s)
        fmt.Println(s)
}
```

Save it and run:

```go
$ go run ints.go 
[1 2 3 4 5 6]
```

## Sort floats

If you have a bunch of floating points instead of integers, you can't use the Ints() method. But the same idea can be used for floats. You use another method Float64s().

```go
package main

import (
	"fmt"
	"sort"
)

func main() {
	s := []float64{7.2, 3.3, 10.7, 13.8, 2.6} // unsorted
	sort.Float64s(s)
	fmt.Println(s)
}
```

Save and run:

```go
$ go run floats.go
[2.6 3.3 7.2 10.7 13.8]
```

**Related links:**
* <a href="https://golang.org/pkg/sort/">The sort package</a>
* <a href="https://golangr.com/">Golang tutorial</a>
