## Getting started
Check go version
```shell
go version
```
Verify environment variables and configuration
```shell
go env
```

1. init go module
```shell
go mod init
```
2. create `hello` directory
3. paste following code to `hellp.go`
```go
package main

import "fmt"

func main() {
	fmt.Println("Hello, World!")
}
```

## Run
- Build & run 
```shell
go build -o hello_build {file_path}
go ./hello_build
```
- Run directly
```shell
go run {file_path}
```

## Managing Dependencies with Go Modules
1. Add new dependency
```shell
go get github.com/labstack/echo/
```

2. Update dependency
```shell
go get -u github.com/labstack/echo/
```

3. Remove unused dependencies
```shell
go mod tidy
```

4. List all dependencies
```shell
go list -m all
```
