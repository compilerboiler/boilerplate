---
title: Golang golang-hello video (snippet)
date: 2019-02-07
tags: ["go"]
---
Go programming example 'golang-hello video'


## golang-hello video

Golang beginners example: golang-hello video

```go
package main

import (
	"gocv.io/x/gocv"
)

func main() {
	webcam, _ := gocv.VideoCaptureDevice(0)
	window := gocv.NewWindow("Hello")
	img := gocv.NewMat()

	for {
		webcam.Read(&img)
		window.IMShow(img)
		if window.WaitKey(1) >= 0 {
			break
		}
	}
}

```

## Useful links

- Learn Go: https://golangr.com
- Download Go: https://golang.org
