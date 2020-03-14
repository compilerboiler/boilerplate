---
tags: ["go"]
date: 2020-02-16
title: what are goroutines
---
---
tags: ["go"]
date: 2020-02-14
title: what are goroutines
---
In programming languages, code is often split up into functions. Functions help to make code reusable, extensible etc. 

In <a href="https://golang.org/">Go</a> there's a special case: goroutines. So is a goroutine a function? Not exactly. A goroutine is a lightweight thread managed by the Go.

If you call a function f like this:

    f(x)

it's a normal function. But if you call it like this:

    go f(x)

it's a goroutine. This is then started <a href="https://golangr.com/concurrency/">concurrently</a>.

If you are new to Go, you can use the <a href="https://play.golang.org/">Go playground</a>

## Goroutine examples

Try this simple program below:

```go
package main

import (
	"fmt"
	"time"
)

func say(s string) {
	for i := 0; i < 3; i++ {
		time.Sleep(100 * time.Millisecond)
		fmt.Println(s)
	}
}

func main() {
	go say("thread")
	say("hello")
}
```

Execute it with:

```
go run example.go
```

So while say('hello') is synchronously executed, go say('hello') is asynchronous.

Consider this program:

```go
package main

import (
    "fmt"
	"time"
)

func main() {
    go fmt.Println("Hi from goroutine")
    fmt.Println("function Hello")
	
    time.Sleep(time.Second) // goroutine needs time to finish
}
```

Then when I ran it:

```
function Hello
Hi from goroutine

Program exited.
```

As expected, the goroutine (thread) started later.

**Related links:**
* <a href="https://golangr.com/goroutines/">More on Goroutines</a>
* <a href="https://golangr.com/">Learn Go</a>

