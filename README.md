[![Build Status](https://api.travis-ci.org/lucazulian/cryptocomparego.svg)](https://travis-ci.org/lucazulian/cryptocomparego)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GoDoc](http://img.shields.io/badge/go-documentation-blue.svg?style=flat-square)](http://godoc.org/github.com/lucazulian/cryptocomparego)
[![Go Report Card](https://goreportcard.com/badge/github.com/lucazulian/cryptocomparego)](https://goreportcard.com/report/github.com/lucazulian/cryptocomparego)
[![Coverage Status](https://coveralls.io/repos/github/lucazulian/cryptocomparego/badge.svg?branch=master)](https://coveralls.io/github/lucazulian/cryptocomparego?branch=master)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/lucazulian/cryptocomparego.svg)](http://isitmaintained.com/project/lucazulian/cryptocomparego "Average time to resolve an issue")
[![Percentage of issues still open](http://isitmaintained.com/badge/open/lucazulian/cryptocomparego.svg)](http://isitmaintained.com/project/lucazulian/cryptocomparego "Percentage of issues still open")

# Cryptocomparego

Cryptocomparego is a Golang client library for accessing the Cryptocompare API.

You can view the client API docs here: [http://godoc.org/github.com/lucazulian/cryptocomparego](http://godoc.org/github.com/lucazulian/cryptocomparego)

You can view Cryptocompare API docs here: [https://www.cryptocompare.com/api/](https://www.cryptocompare.com/api/)


## Usage

```go
import "github.com/lucazulian/cryptocomparego"
```

## Examples


To get general info for all the coins available:

```go
ctx := context.TODO()

client := NewClient(nil)
coinList, _, err := client.Coin.List(ctx)

if err != nil {
    fmt.Printf("Something bad happened: %s\n", err)
    return err
}
```

## Contributing

We love pull requests! Please see the [contribution guidelines](CONTRIBUTING.md).
