## Dependencies

- [Go](https://go.dev/dl/)
- [Protocol buffer compiler](https://protobuf.dev/installation/)
- Go plugins:

```
go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest
```

## Compiling from .proto to .go

```
protoc --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative ./queen_ant.proto
```
