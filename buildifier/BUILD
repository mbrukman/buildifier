load("@io_bazel_rules_go//go:def.bzl", "go_binary")

go_binary(
    name = "buildifier",
    srcs = ["buildifier.go"],
    visibility = ["//visibility:public"],
    deps = [
        "//core:go_default_library",
        "//differ:go_default_library",
    ],
)
