---
title: Golang golang-json2 (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-json2'


## golang-json2

Golang beginners example: golang-json2

```go
package main

import (
	"bytes"
	"encoding/json"
	"fmt"
	"io"
	"strings"
)

const jsonString = `
	[
		{
			"type": "group",
			"value": [
				"Lorem",
				"Ipsum",
				"dolor",
				"sit",
				"Amet"
			]
		},
		{
			"type": "value",
			"value": "Hello World"
		},
		{
			"type": "value",
			"value": "foobar"
		}
	]
`

type Codec interface {
	Encode(w io.Writer, v interface{}) error
	Decode(r io.Reader, v interface{}) error
}

type jsonCodec struct{}

func (*jsonCodec) Encode(w io.Writer, v interface{}) error {
	return json.NewEncoder(w).Encode(v)
}
func (*jsonCodec) Decode(r io.Reader, v interface{}) error {
	return json.NewDecoder(r).Decode(v)
}

func trimByte(str *bytes.Buffer) string {
	return strings.TrimSpace(fmt.Sprint(str))
}

var JSON Codec = (*jsonCodec)(nil)

func main() {
	var m interface{}
	var b bytes.Buffer

	fmt.Printf("INPUT: %s\n", jsonString)

	if err := JSON.Decode(strings.NewReader(jsonString), &m); err == nil {
		fmt.Printf("DECODED: %#v\n", m)
	} else {
		fmt.Println(err)
	}

	if err := JSON.Encode(&b, &m); err == nil {
		fmt.Printf("ENCODED: %s\n", trimByte(&b))
	} else {
		fmt.Println(err)
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
