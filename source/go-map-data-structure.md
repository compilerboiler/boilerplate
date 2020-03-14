<a href="https://golang.org">Go</a> comes with many data structures, including a <a href="https://golangr.com/maps/">map</a> data structure.

A (hash)map maps keys to values, this is a common data structure in programming. Many languages support it including Go and Python (dictionary).

Unlike an array, it has a one to one mapping. The key can be used to quickly get the value without using a loop

```go
m["Cat"] = "Meow"
fmt.Println(m["Cat"])
```

Above the key is "Cat" and the value is "Meow", which is then returned.


## Introduction

You can use the **make()** function to create a map. If you call the make() function is returns a map initialized and ready for use.

In Go it's important to define the data types of the key and the value.
You can create all kind of maps, like a string to string mapping.

Example, map a key to a value where both are <a href="https://golangr.com/strings/">strings</a>

```go
var m map[string]string

// map key (string) to value (string)
m = make(map[string]string)
```

Go lets you map a key to value, where the value is an integer (int64):

```go
var m map[string]int64

// map key (string) to value (integer)
m = make(map[string]int64)
```

![hashmap](https://dev-to-uploads.s3.amazonaws.com/i/ykbjcnrkbfunucryhxox.png)

## Go Map Example

The example below creates a map (string -> string), sets a key pair and returns a value using a key. The **map** function makes the map. Then one (key,value) pair is set.

```go
package main

import "fmt"

var m map[string]string

func main() {
	m = make(map[string]string)
	m["Cat"] = "Meow"
	fmt.Println(m["Cat"])
}
```

The output of the above program is

    Meow
    
    Program exited.

So the value was given for the key "Cat", the key pair is ("Cat","Meow").

An example of a key-value mapping with integers, where there are multiple items. The **map** function is used to initialize the map.

```go
package main

import "fmt"

var m map[string]int64

func main() {
	m = make(map[string]int64)
	m["Serge"] = 33
	m["Thomas"] = 25
	m["Juan"] = 28
	fmt.Println(m["Serge"])
}
```

This program outputs:

    33

    Program exited.


