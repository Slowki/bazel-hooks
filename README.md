# bazel-hooks

[`pre-commit`](https://pre-commit.com/) hooks to run [Buildifier](https://github.com/bazelbuild/buildtools/tree/master/buildifier).

## Buildifier Hook

### Using the System version of Buildifier

```yaml
repos:
  - repo: https://github.com/Slowki/bazel-hooks
    rev: 06fa15336c55bd35ac5abd77a42d24bdb005151c
    hooks:
      - id: buildifier
```

### Using Buildifier via Bazel

`bazel-buildifier` runs the `@com_github_bazelbuild_buildtools//buildifier` target.

```yaml
repos:
  - repo: https://github.com/Slowki/bazel-hooks
    rev: 06fa15336c55bd35ac5abd77a42d24bdb005151c
    hooks:
      - id: bazel-buildifier
```
