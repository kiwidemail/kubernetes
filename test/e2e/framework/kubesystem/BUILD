load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["kubesystem.go"],
    importpath = "k8s.io/kubernetes/test/e2e/framework/kubesystem",
    visibility = ["//visibility:public"],
    deps = [
        "//test/e2e/framework:go_default_library",
        "//test/e2e/framework/ssh:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
