---
title: Golang golang-command line arguments (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-command line arguments'


## golang-command line arguments

Golang beginners example: golang-command line arguments

```go
package main

import (
	"flag"
	"fmt"
)

func main() {
	env := flag.String("env", "dev", "Environment(dev, qa, stg, prod)")
	cron := flag.Bool("consumer", false, "boolean")
	//Parse parses the command-line flags
	flag.Parse()
	fmt.Println("The environment set is", *env)
	fmt.Println("The consumer flag retrieved from command line is", *cron)
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
