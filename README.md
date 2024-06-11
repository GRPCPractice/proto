# Setup
```shell
go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.28
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.2
brew install protobuf
```

# How to use
## Generate proto files 
```shell
protoc --go_out=. --go-grpc_out=. -Iproto proto/helloworld/helloworld.proto
protoc --go_out=. --go-grpc_out=. -Iproto proto/user/user.proto
```

## Go get
```shell
go get github.com/GRPCPractice/proto
```

## Add submodule
```shell
git submodule add https://github.com/GRPCPractice/proto.git proto
```