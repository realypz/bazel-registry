# Bazel Registry

This repo defines the dependencies not existing in Bazel registry yet.

To use this customized registry, add following content to your project's `.bazelrc`.

```txt
common --registry=https://bcr.bazel.build  # The Bazel Central Registry
common --registry=https://raw.githubusercontent.com/realypz/bazel-registry/main
```

If you wants to use a local registry instead, then use the following content in `.bazelrc`.

```txt
common --registry=file://<path>/<bazel-registry-repo>
```

## References

[Bazel Registries](https://bazel.build/external/registry)
