---
title: Golang golang-json (snippet)
date: 2020-02-08
tags: ["go"]
---
Go programming example 'golang-json'


## golang-json

Golang beginners example: golang-json

```go
package main

import (
	"encoding/json"
	"fmt"
	"os"
)

//var strings = []string{"lorem", "ipsum", "dolor", "sit", "amet"}

func main() {

	var strings []string
	var jsonstring = `["lorem", "ipsum", "dolor", "sit", "amet"]`

	//convert json bytes-string to object
	err := json.Unmarshal([]byte(jsonstring), &strings)

	if err != nil {
		fmt.Println("error while unmarshalling")
		os.Exit(2)
	}

	fmt.Println(strings)

	//convert object to bytes-string
	jsonData, err := json.Marshal(strings)

	if err != nil {
		fmt.Println("error while marshalling")
		os.Exit(2)
	}

	fmt.Println(string(jsonData))
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
