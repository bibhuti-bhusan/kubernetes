load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["types.go"],
    importmap = "k8s.io/kubernetes/vendor/github.com/heketi/heketi/pkg/glusterfs/api",
    importpath = "github.com/heketi/heketi/pkg/glusterfs/api",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/go-ozzo/ozzo-validation:go_default_library",
        "//vendor/github.com/go-ozzo/ozzo-validation/is:go_default_library",
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
