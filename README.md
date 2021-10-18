<h1 align="center">
  go-safestr
</h1>

<p align="center">
  A library to get safe strings for <a href="https://golang.org/">Golang</a>
</p>

<p align="center">
  <a href="https://travis-ci.com/blacktrue/go-safestr"><img src="https://travis-ci.com/blacktrue/go-safestr.svg?branch=master"></a>
  <a href="https://codecov.io/gh/blacktrue/go-safestr">
    <img alt="Coverage" src="https://codecov.io/gh/blacktrue/go-safestr/branch/master/graphs/badge.svg?branch=master">
  </a>
</p>

This package provides a function to parse string to safe string adding replacement values, please fork and [create](https://github.com/blacktrue/go-safestr/pulls) a pull request.

# Installation
```
$ go get -u github.com/blacktrue/go-safestr/
```

# Usage
```go
import (
	"log"
	"github.com/blacktrue/go-safestr"
)

parsedValue, err := Parse('1232124543233254', '*', 4)
if err != nil {
	log.Println(err.Error())
}

log.Println(*parsedValue)
```

## Functions
You can call these functions from your application.

| Function                                                  | Has Params |
| --------------------------------------------------------- | ---------- |
| Parse(value string, replacement string, visible int)                                      | Yes |
