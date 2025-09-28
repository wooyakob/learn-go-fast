.DEFAULT_GOAL := build

.PHONY: fmt vet build clean

fmt:
	go fmt ./...
vet:
	go vet ./...
build: vet
	go build
clean:
	go clean
	rm -f hello_world go-programs *.out *.test

