# About

This project contains BUILD files to compile and use the [C++ driver for MongoDB](https://github.com/mongodb/mongo-cxx-driver) with Bazel, using [rules_foreign_cc](https://github.com/bazelbuild/rules_foreign_cc).

# How to run

You can run the tutorial code with mongocxx with the command `bazel run tutorial`. This assumes you have [bazelisk](https://github.com/bazelbuild/bazelisk) installed and symlinked as "bazel".

If you want to use the mongocxx driver in your own Bazel project, you can import the BUILD files and depend on it like done here:
```starlark
deps = ["@mongocxx"],
```

Please keep in mind the compilation options that have been applied might not be the ones you need or prefer. This BUILD files produce statically linked versions of the libraries only.
