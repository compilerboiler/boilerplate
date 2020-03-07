---
title: Golang golang-codegen (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-codegen'


## golang-codegen

Golang beginners example: golang-codegen

```go
package main

import (
	"encoding/json"
	"os"
	"reflect"
	"strings"
	"text/template"
)

//go:generate go run codegen.go
//go:generate go fmt codegenerated/codegenerated.go

type Struct struct {
	Name   string
	Fields map[string]interface{}
}

func title(input string) string {
	input = strings.Replace(input, "_", " ", -1)
	input = strings.Title(input)
	input = strings.Replace(input, " ", "", -1)
	return input
}

func typeOf(v interface{}) string {
	if v == nil {
		return "string"
	}
	return strings.ToLower(reflect.TypeOf(v).String())
}

func genStructCode() {
	templateString, jsonString := getExampleData()

	var resp map[string]interface{}
	json.Unmarshal([]byte(jsonString), &resp)

	data := Struct{"Data", resp}

	tpl, _ := template.New("struct").Funcs(template.FuncMap{
		"Title":  title,
		"TypeOf": typeOf,
	}).Parse(templateString)

	out, _ := os.Create("codegenerated/codegenerated.go")
	defer out.Close()

	tpl.Execute(out, data)
}

func main() {
	genStructCode()
}

func getExampleData() (string, string) {
	templateString := `
package codegen

type {{ .Name | Title }} struct {
{{ range $jsonName, $val := .Fields }}
    {{- $jsonName | Title }} {{ $val | TypeOf }} ` + "`" + `json:"{{ $jsonName }}"` + "`" + `
{{ end }}
}
`

	jsonString := `
{
  "lorem": "ipsum",
  "dolor": "sit",
  "amet": 1337,
  "foo_bar": true,
  "bar": false
}
`
	return templateString, jsonString
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
