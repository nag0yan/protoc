FROM "mcr.microsoft.com/devcontainers/go:1-1.21-bullseye"


RUN apt-get update && export DEBIAN_FRONTEND=noninteractive

# install formatter for proto3
RUN apt-get -y install clang-format

# install gRPC tools
RUN go get google.golang.org/protobuf/cmd/protoc-gen-go \
    && go install google.golang.org/protobuf/cmd/protoc-gen-go \
    && go get google.golang.org/grpc/cmd/protoc-gen-go-grpc \
    && go install google.golang.org/grpc/cmd/protoc-gen-go-grpc
