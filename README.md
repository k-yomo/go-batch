[![License: BSD 3-Clause](https://img.shields.io/badge/License-BSD--3--Clause-blue.svg)](https://github.com/k-yomo/go-batch/blob/main/LICENSE)
[![Main Workflow](https://github.com/k-yomo/go-batch/actions/workflows/test.yml/badge.svg)](https://github.com/k-yomo/go-batch/actions/workflows/test.yml)
[![codecov](https://codecov.io/gh/k-yomo/go-batch/branch/main/graph/badge.svg)](https://codecov.io/gh/k-yomo/go-batch)
[![Go Report Card](https://goreportcard.com/badge/github.com/k-yomo/go-batch)](https://goreportcard.com/report/github.com/k-yomo/go-batch)

# go-batch
Type-safe batching library for Go with 1.18+ Generics forked from [google.golang.org/api/support/bundler](https://pkg.go.dev/google.golang.org/api/support/bundler).

## Installation
```shell
$ go get -u github.com/k-yomo/go-batch
```

## Example
```go
batcher := batch.New(func (items []int) {
	fmt.Printf("%+v", items)
})

batcher.Add(1, 1)
```
