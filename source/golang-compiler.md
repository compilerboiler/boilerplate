If you have the <a href="https://golang.org/">Go programming language</a> installed on your computer, you can run Go programs. You can verify this by opening a terminal and typing 

```
go version
```

If it outputs an error like "command not found", you should <a href="https://golangr.com/install/">install</a> it. 


Then you can save your program as filename.go (the .go extension) and run it with:

```
go run filename.go
```

That then runs the program and outputs it in the terminal. What if you want to have a program?

Then you have to <a href="https://en.wikipedia.org/wiki/Compiler">compile</a> it. Compiling converts your source code into an actual program.

## Compile in Go

You can do so in a few steps. Open up a terminal (On Linux: Ctrl+Alt+t).
First create new directory for your project:

```bash
➜  ~ mkdir hello
➜  ~ cd hello
```

Now create your <a href="https://golangr.com/hello-world/">hello world</a> program with your favorite editor.

```
➜  hello vim hello.go
```

Do note I'm using a <a href="https://ohmyz.sh/">Zsh</a> theme so it puts the directory name in front. 
The hello world program:

```go
package main

import "fmt"

func main() {
	fmt.Println("Hello, world.")
}
```

Save it and exit the editor.
Now you can run the build command:

```
➜  hello go build hello.go
```

And you have an application that you can run

```
➜  hello ./hello
Hello, world.
```

That's it! Simple
