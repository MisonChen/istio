load("@io_bazel_rules_go//go:def.bzl", "go_binary", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["main.go"],
    visibility = ["//visibility:public"],
    deps = [
        "//security/cmd/node_agent/na:go_default_library",
        "//security/pkg/cmd:go_default_library",
        "@com_github_coreos_go_oidc//:go_default_library",
        "@com_github_golang_glog//:go_default_library",
        "@com_github_spf13_cobra//:go_default_library",
        "@org_golang_x_net//context:go_default_library",
    ],
)

go_binary(
    name = "node_agent",
    library = ":go_default_library",
    visibility = ["//visibility:public"],
)
