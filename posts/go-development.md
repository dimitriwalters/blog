---
title: 'How to get started with Go development'
date: '2024-10-07'
---

Go is actually the easiest language in my experience to get started with. You don't need an IDE or third-party tool to setup package management; everything is built into go once you install it:

```
brew install go
```

[(or a similar installation)](https://go.dev/doc/install)

Whenever you need to use a third-party package your simply run

```
go get github.com/gorilla/mux
```

This installs packages in your `$GOPATH`. And even if you forget to run these commands the compiler will tell you to do so anyways.

To use a package you import it at the beginning of you file:

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

All of these are from standard library (which will probably be sufficient for 95% of code you write); also it's in alphabetical order by convention.

This guide should get you started with running some Go code. Next blog will get into Go primitive types and operations, and after that concurrency.