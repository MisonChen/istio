load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "externs.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//mixer/pkg/expr:go_default_library",
        "//mixer/pkg/il/interpreter:go_default_library",
        "@io_istio_api//:mixer/v1/config/descriptor",
    ],
)

go_test(
    name = "go_default_test",
    size = "small",
    srcs = [
        "externs_test.go",
    ],
    library = ":go_default_library",
)
