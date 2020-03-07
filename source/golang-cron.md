---
title: Golang golang-cron (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-cron'


## golang-cron

Golang beginners example: golang-cron

```go
package main

import (
	"fmt"
	"github.com/robfig/cron"
	"time"
)

func main() {
	c := cron.New()
	MinuteCheck := time.Now().Minute() + 1
	SpecVal := fmt.Sprintf("%d", MinuteCheck) + " * * * *"
	fmt.Println("The SpecVal is ", SpecVal)
	_, err := c.AddFunc(SpecVal, PrintNumber)
	if err != nil {
		fmt.Println("Could not register cron - PrintNumber. Error:", err)
	}
	c.Start()
	time.Sleep(time.Second * 70)
}

func PrintNumber() {
	fmt.Println("The function was triggered at time:", time.Now())
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
