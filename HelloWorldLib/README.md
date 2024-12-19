# emscripten

    mkdir out

    emcc -o out/Lib.o -c Lib.c
    emar rcs out/Lib.a out/Lib.o

    emcc -o out/App.wasm App.c out/Lib.a

    wasmtime run out/App.wasm
