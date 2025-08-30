# emscripten

## generate html, js, and wasm

    mkdir out

    emcc -o out/HelloWorld.html HelloWorld.c -s PURE_WASI

1. Without `-s PURE_WASI`, `wasmtime` does not print anything.


# run

## browser

    python3 -m http.server 8080 --dir out

    open http://localhost:8080/HelloWorld.html

## node

    node out/HelloWorld.js

## wasmtime

    wasmtime run out/HelloWorld.wasm

## native

    cc -o out/HelloWorld HelloWorld.c
    out/HelloWorld
