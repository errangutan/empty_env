load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

git_repository(
    name = "meru",
    branch = "master",
    remote = "git@github.com:errangutan/meru.git",
)

load("@meru//:meru_deps.bzl", "meru_deps")
meru_deps()
