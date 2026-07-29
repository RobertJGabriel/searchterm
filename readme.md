# searchterm

> A minimal Go HTTP server that echoes back the query parameters it receives.

Starts a server on port `9094`, parses the form and query values of every
incoming request, logs them, and replies with a fixed string.

This is a learning exercise following the HTTP chapter of
*Build Web Application with Golang* — hence the `Hello astaxie!` response left in
the handler. Despite the repository name, it does **not** extract search terms
from URLs.

## Requirements

Go.

## Usage

```sh
go run main.go
```

Then send it a request:

```sh
curl 'http://localhost:9094/?url_long=https://www.google.com/search?q=golang'
```

The query keys and values are printed to the server's stdout. The response body
is always `Hello astaxie!`.

## Status

A scratch exercise, kept for reference. Not maintained, and not a usable package.

## License

No licence file. All rights reserved unless stated otherwise.
