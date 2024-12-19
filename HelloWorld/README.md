# emscripten

## generate html, js, and wasm

    mkdir out

    emcc -o out/HelloWorld.html HelloWorld.c -s PURE_WASI

## run html

    python3 -m http.server 8080 --dir out

1. Open http://localhost:8080/HelloWorld.html in a browser

## run js

    node out/HelloWorld.js

## run wasm

    wasmtime run out/HelloWorld.wasm


# native

    cc -o out/HelloWorld HelloWorld.c
    out/HelloWorld
