workspace(name = "rules_ksonnet")

git_repository(
    name = "io_bazel_rules_go",
    remote = "https://github.com/bazelbuild/rules_go.git",
    tag = "0.5.0",
)

load("@io_bazel_rules_go//go:def.bzl", "go_repositories")

go_repositories()

load("//:rules.bzl", "ksonnet_repositories", "kubecfg_repositories")

kubecfg_repositories()

ksonnet_repositories()
