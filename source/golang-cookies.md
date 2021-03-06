---
title: Golang golang-cookies (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-cookies'


## golang-cookies

Golang beginners example: golang-cookies

```go
package main

import (
	"fmt"
	"log"
	"net/http"
	"strconv"
	"time"
)

func rootHandler(w http.ResponseWriter, r *http.Request) {
	c, err := r.Cookie("timestamp")
	cookie := &http.Cookie{
		Name:  "timestamp",
		Value: strconv.FormatInt(time.Now().Unix(), 10),
	}
	http.SetCookie(w, cookie)
	if err != nil {
		fmt.Println(err)
		fmt.Fprintf(w, "Hello, you're here for the first time")
	} else {
		timeint, _ := strconv.ParseInt(c.Value, 10, 0)
		fmt.Fprintf(w, "Hi, your last visit was at "+time.Unix(timeint, 0).Format("15:04:05"))
	}
}

func main() {
	http.HandleFunc("/", rootHandler)
	log.Fatal(http.ListenAndServe(":8080", nil))
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
