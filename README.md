# golearn

## First usage (To enable usage in Terminal mode)
- Init **Go Mod** in this project:
    - initialize a v0 or v1 module: `go mod init example.com/m`, or
    - initialize a v2 module: `go mod init example.com/m/v2`, or
    - any version you like
- Add module requirements and sums: `go mod tidy`
- `go install` Command will compile and stored the results into `~/go/bin/<here>` directory
- While `go build` will compile it into binary a file and be stored in the same location with the original ***.go** file

## Install Go codes using `go install` (compiled and copied into `~/go/bin/` directory)
- Sample usage (Hello world)
        1. Go to `./code_examples/01_hello_world` directory, to locate `main.go` file
        2. Run command: `go install`
        3. Compiled file is stored in `~/go/bin/01_hello_world` (**Executable, 1.8MB**)
        4. To run it, execute: `~/go/bin/01_hello_world main.go`

## Building Go using `go build` (built into a binary file)
- Sample usage (Hello world)
    1. Go to `./code_examples` directory, to locate `01_hello_world.go` file
    2. Run command: `go build`
    3. Compiled binary file is stored in `./01_hello_world` (same directory)
    4. To run it, execute: `~/go/bin/code_examples 01_hello_world.go`

## Learning materials
1. [Hello world](https://golangbot.com/hello-world-gomod/)

## MISC
- [Go package download](https://golang.org/dl/)
- [Go Installation](https://golang.org/doc/install)
- Set Go $PATH permanently in [Fish Shell](https://github.com/fish-shell/fish-shell) (Do it only ONCE):
    `$ set -Ua fish_user_paths /usr/local/go/bin`