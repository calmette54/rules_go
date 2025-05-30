# rules_go "Hello World" example

This directory contains a minimal, standalone example using Bazel and rules_go. It shows how to use the [`go_binary`](../../go/core/rules.md#go_binary), [`go_library`](../../go/core/rules.md#go_library), and [`go_test`](../../go/core/rules.md#go_test) rules without requiring any other dependencies.

Jump into the development environment:

```bash
nix develop
```

To run the binary:

```bash
bazelisk run //:hello --shell_executable=$(which bash)
```

To test the library:

```bash
bazelisk test //:hello_test --shell_executable=$(which bash)
```

For an explanation and an introduction to Bazel, see [Bazel Tutorial: Build a Go Project](https://bazel.build/start/go).
