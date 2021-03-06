---
title: Golang golang-httpd (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-httpd'


## golang-httpd

Golang beginners example: golang-httpd

```go
package main

import (
	"fmt"
	"log"
	"net/http"
	"strconv"
	"strings"
)

var requestcounter int

func handler(w http.ResponseWriter, r *http.Request) {
	url := r.URL.Path
	if r.URL.RawQuery != "" {
		url = strings.Join([]string{url, "?", r.URL.RawQuery}, "")
	}
	fmt.Fprintf(w, "Hello World\nYou requested: %s\n", url)
	fmt.Fprintf(w, "this is request number %s\n", strconv.Itoa(requestcounter))
	log.Println(url)
	requestcounter++
}

func main() {
	http.HandleFunc("/", handler)
	err := http.ListenAndServe(":8080", nil)
	if err != nil {
		log.Fatal("ListenAndServe: ", err)
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
