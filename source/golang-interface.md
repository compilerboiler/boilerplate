---
title: Golang golang-interface (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-interface'


## golang-interface

Golang beginners example: golang-interface

```go
package main

import (
	"fmt"
	"time"
)

func String(value interface{}) string {
	switch val := value.(type) {
	case bool:
		if value.(bool) == true {
			return "true"
		}
		return "false"
	case time.Duration:
		return string(val.String())
	case time.Time:
		return string(val.Format(time.RFC3339))
	case string:
		return val
	case []byte:
		return string(val)
	default:
		return fmt.Sprintf("%v", val)
	}
}

func main() {
	fmt.Println(String(0x23))
	fmt.Println(String(0xfefe))
	fmt.Println(String(time.Minute * 5))
	fmt.Println(String(time.Now()))
	fmt.Println(String(false))
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
