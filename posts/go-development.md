---
title: 'How to get started with Go development'
date: '2024-10-07'
---

Go is actually the easiest language in my experience to get started with. You don't need an IDE or third-party tool to setup package management; everything is built into go once you install it:

```
brew install go
```

[(or a similar installation)](https://go.dev/doc/install)

Whenever you need to use a third-party package you simply run

```
go get github.com/gorilla/mux
```

This installs packages in your `$GOPATH`. If you forget to run these commands the compiler will reminder you to do so.

To use a package you import it at the beginning of your file:

```
import (
    "context"
    "errors"
    "fmt"
    "io"
    "net/http"
    "os"
)
```

In this case, all of these imports are from standard library (which will be sufficient for a lot of code you write); the packages are also listed in alphabetical order by convention.

This guide should get you started with running some Go code. Next topic will get into Go primitives and concurrency.