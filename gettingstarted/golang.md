# The Go Programming Language

One of our primary languages is the
[Go (AKA Golang) programming language](https://golang.org/). In Otrego we will
largely use the term "Golang" as opposed to "Go", to avoid ambiguity with the
game.

## Installing

*   [Download from the Golang Website](https://golang.org/dl/)
*   If you are on OSX, you can also install with [homebrew](https://brew.sh/)


## Learning Golang

Golang has fantastic getting started materials:

1.  [Getting Started with Go](https://golang.org/doc/tutorial/getting-started)
2.  [The Go Tour](https://tour.golang.org/welcome/1)
3.  [How to Write Go Code](https://golang.org/doc/code.html)
4.  [Go Docs Collection on golang.org](https://golang.org/doc/)
5.  [Go By Example](https://gobyexample.com/) -- Learning Golang by examples.
6.  [The Go Programming Language (Book)](https://www.gopl.io/) -- The best
    book on the Go programming language.

### Installing Tools

We use golint for linting our go-files.

```shell
go get -u golang.org/x/lint/golint
```

## Workflows

### Building and Testing

Make sure the repository builds, assuming you're in `clamshell` repository or
some othe other repository that uses Golang:

Build the sources:

```shell
# Build current package (current directory)
go build

# Build all packages recursively
go build  ./...
```

Build & test the sources:

```shell
# Build and test current package (current directory)
go test ./...

# Test all packages recursively
go test ./...
```

### Ensuring Code Qualiy

Make sure your code is formatted:

```shell
# Format current package.
go fmt
```

Ensure go code quality by using go vet and golint.

```shell
golint ./...
go vet ./...
```

### Other Resources

*   **Effective Go**: https://golang.org/doc/effective_go -- Style guide & Best
    practices for Go.
*   **Code Review Comments**:
    https://github.com/golang/go/wiki/CodeReviewComments -- Common style
    recommendations that come up in code review.
