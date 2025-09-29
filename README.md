# learn-go-fast

properly written, go is boring.

invented at Google to address issues with C++ and Java

* slow compilation
* complex dependency management
* poor support for modern multicore, networked systems

there is now a strategy that allows Go to keep backward compatibility required for long term software projects, whilst providing the ability to address backward breaking changes to address long standing design flaws.

Go is often used to build and call HTTP servers.

Download ARM64 https://go.dev/dl/

*Brew install go*

*wooyakob@Mac learn-go-fast % go version
go version go1.25.1 darwin/arm64*

mark directory as a go module

go mod init

enable telemetry

go run golang.org/x/telemetry/cmd/gotelemetry@latest on

view collected data at [telemetry.go.dev](https://telemetry.go.dev/ "https://telemetry.go.dev")

or preview with go run golang.org/x/telemetry/cmd/gotelemetry@latest view

learn: https://go.dev/learn/

go projects are called modules

a module is not just source code. it is an exact specification of the dependencies of the code within the module.

go.mod - includes minimum supported version of go for the module, go1.25.1

similar to requirements.txt file in python - go.mod

use go mod

and go tidy

to make changes to file, never directly

go build

creates an executable

go defines a standard way of formatting

go fmt auto fixes whitespace to auto format

go.fmt

to format program

run go vet to scan for code erros

makefiles

modern software, repeatable automatable builds run by anyone, anywhere

default goal - target run when none specified

ensuring formatting

and vetting

before a dev triggers a build

predeclared types and declarations:

write your programs in a way that makes your intentions clear

predeclared types

- zero value - default zero value to any variable that is declared but not assigned a value
- literals - explicitly specified number, char or string
-
