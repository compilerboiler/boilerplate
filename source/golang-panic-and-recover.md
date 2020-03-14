In <a href="https://golang.org/">Golang</a>, Panic is a function that stops the ordinary flow of control and starts panicking.

<a href="https://golangr.com/errors/">Errors</a> are for abnormal conditions during program execution, but there are some cases where the program cannot continue executing after something went wrong.

In that case you can use panic to terminate the program.

A simple example is creating a new file, which is a requirement of the program. If the file cannot be created, the control flow must stop:

```go
    _, err := os.Create("/tmp/file")
    if err != nil {
        panic(err)
    }
```

## Example

The program below demonstrates the use of panic(). A program calls a function sayHello(name), which on normal situations outputs the name.

But what if a name is not specified? Then something went wrong: panic.

```go
package main

import (  
    "fmt"
)

func sayHello(name *string) {  
    if name == nil {
        panic("runtime error: name cannot be nil")
    }
    fmt.Printf("Hello %s\n", *name)
}

func main() {  
    sayHello(nil)
}
```

This outputs in the terminal:

```go
➜  ~ go run pan.go 
panic: runtime error: name cannot be nil

goroutine 1 [running]:
main.sayHello(...)
        /home/frank/pan.go:9
main.main()
        /home/frank/pan.go:15 +0x3a
exit status 2
```

## Recover

If the *panic* situation happens, the program terminates. In the real world, this is not good. 

The application terminating on error? Nobody wants that. Instead, you need a mechanism to recover from the error.

```bash
This is a Panic Situation
Recovery function
Main block executed
```

In code that looks like this:

```go
package main

import (
    "fmt"
)

func makePanic() {
    defer recoveryFunction()
    panic("This is a Panic Situation")
}

func recoveryFunction() {
    if recoveryMessage := recover(); recoveryMessage != nil {
      fmt.Println(recoveryMessage)
    }
    fmt.Println("Recovery function")
}

func main() {
    makePanic()
    fmt.Println("Main block executed")
}
```

**Related links:**
* <a href="https://golang.org/">Golang official website</a>
* <a href="https://golangr.com/">Learn Golang</a>



