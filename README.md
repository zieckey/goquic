# goquic

Chromium QUIC protocol implementation binding for Go

# How to build

Due to cgo restrictions, use an environment variable like below to build your projects.

    CGO_LDFLAGS="-L$GOPATH/src/github.com/devsisters/goquic/lib/$GOOS_$GOARCH"

For example, building gospdyquic example server in mac:

    CGO_LDFLAGS="-L$GOPATH/src/github.com/devsisters/goquic/lib/darwin_amd64" go build github.com/devsisters/gospdyquic/example
