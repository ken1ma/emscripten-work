# Environment

1. emscripten 4.0.13, node 24.7.0

       brew install emscripten

       emcc --version
       node --version

1. wasmtime 36.0.2

       curl https://wasmtime.dev/install.sh --silent --show-error --fail | bash

       wasmtime --version

    1. This script installs into `$WASMTIME_HOME` (defaults to `$HOME/.wasmtime`)
    1. This script modifies into `$HOME/.bash_profile`
