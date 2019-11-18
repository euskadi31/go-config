Go Config [![Last release](https://img.shields.io/github/release/euskadi31/go-config.svg)](https://github.com/euskadi31/go-config/releases/latest) [![Documentation](https://godoc.org/github.com/euskadi31/go-config?status.svg)](https://godoc.org/github.com/euskadi31/go-config)
====================

[![Go Report Card](https://goreportcard.com/badge/github.com/euskadi31/go-config)](https://goreportcard.com/report/github.com/euskadi31/go-config)

| Branch  | Status | Coverage |
|---------|--------|----------|
| master  | [![Build Status](https://img.shields.io/travis/euskadi31/go-config/master.svg)](https://travis-ci.org/euskadi31/go-config) | [![Coveralls](https://img.shields.io/coveralls/euskadi31/go-config/master.svg)](https://coveralls.io/github/euskadi31/go-config?branch=master) |


Simple Config library for Golang

/!\ Work In Progress /!\

## Example

```go
package main

import (
    "fmt"
    "github.com/euskadi31/go-config"
)

type AppConfiguration struct {
    Name string
}

type Configuration struct {
    App *AppConfiguration
}

func main() {
    var cfg *Configuration

    if err := config.Unmarshal(&cfg); err != nil {
        panic(err)
    }
}

```

## License

go-config is licensed under [the MIT license](LICENSE.md).
