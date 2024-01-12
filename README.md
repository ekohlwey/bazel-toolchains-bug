# Bazel Toolchains Declaration Bug Example

This is an example repository for a bug I reported to the bazel project.

This project contains a single build target for a toolchain (`//:java_toolchain`).

The failing commit appears to be https://github.com/bazelbuild/bazel/commit/30d033cd7e2153e8b8d7eb034a5323053192ecaa

You can find the failure using `bazelisk --bisect=6.4.0..7.0.0 build //:java_toolchain`.
