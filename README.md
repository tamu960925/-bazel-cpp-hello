# Bazel C++ Hello, World

Minimal Bazel + C++ project that prints "Hello, Bazel!".

## Prerequisites
- Bazel (or Bazelisk)
- C++ toolchain (`clang` or `g++`)

On macOS, you can install Bazelisk:
```bash
brew install bazelisk
```

## Build
```bash
bazel build //:hello_world
```

## Run
```bash
bazel run //:hello_world
# Expected output:
# Hello, Bazel!
```

## Clean
```bash
bazel clean
```

## Files
- `WORKSPACE` — empty workspace definition
- `BUILD` — `hello_world` binary rule
- `main.cc` — prints the greeting

