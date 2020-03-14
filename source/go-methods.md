<a href="https://golang.org/">Go</a> does not have classes or object orientated programming in the traditional sense. But you can define methods on types.

In Go, a method is a function with a special receiver argument. For example, we define two methods like that (getX and getY):

```go
package main

import (
	"fmt"
)

type Coordinate struct {
	X, Y float64
}

func (v Coordinate) getX() float64 {
	return v.X
}

func (v Coordinate) getY() float64 {
	return v.Y
}

func main() {
	v := Coordinate{3, 4}
	fmt.Println(v.getX())
	fmt.Println(v.getY())
}
```

This outputs the x and y values of the struct.

```go
3
4

Program exited.
```

So on a programming level with Go, you might not miss OOP as <a href="https://golangr.com/struct/">structs</a> work just fine and you can apply methods.

A method can do more than just return a value. In the example below, the method Abs has a receiver of type Vertex named v.

```go
package main

import (
	"fmt"
	"math"
)

type Vertex struct {
	X, Y float64
}

func (v Vertex) Abs() float64 {
	return math.Sqrt(v.X*v.X + v.Y*v.Y)
}

func main() {
	v := Vertex{3, 4}
	fmt.Println(v.Abs())
}
```
