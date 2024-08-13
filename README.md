# WasmEdge WASI Socket Http Server Demo

This demo runs an echo server on `localhost`.

## Build

```shell
cargo build --target wasm32-wasi --release
```

## Run

```shell
wasmedge target/wasm32-wasi/release/http_server.wasm
```

## Test

In another terminal window, do the following.

```shell
curl -X POST http://127.0.0.1:1234 -d "name=WasmEdge"
echo: name=WasmEdge
```

# LICENSE

Apache-2.0license

This repository is from [second-state/wasmedge_wasi_socket](https://github.com/second-state/wasmedge_wasi_socket/tree/main), which is under Apache-2.0license.
