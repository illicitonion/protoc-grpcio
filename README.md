# grpcio-compiler-protoc
[![Build Status](https://travis-ci.org/mtp401/protoc-grpcio.svg?branch=master)](https://travis-ci.org/mtp401/protoc-grpcio)

A programmatic API to the
[grpc-rs compiler](https://github.com/pingcap/grpc-rs).

## Example

```rust
extern crate grpcio_compiler_protoc;

grpcio_compiler_protoc::compile_grpc_protos(
    &["example/protobuf.proto"],
    &["example"],
    "output"
).expect("failed to compile gRPC definitions");

```

## Credits

Credit to both the TiKV project developers for
([grpc-rs](https://github.com/pingcap/grpc-rs)) and Stepan Koltsov
(@stepancheg, [rust-protobuf](https://github.com/stepancheg/rust-protobuf))
for their amazing work bringing Protocol Buffers and gRPC support to Rust.
