package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["options.go"],
    importpath = "k8s.io/kubernetes/federation/cmd/federation-controller-manager/app/options",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/spf13/pflag:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//cmd/vendor/k8s.io/apiserver/pkg/util/flag:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/federation/pkg/dnsprovider:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/apis/componentconfig:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/client/leaderelectionconfig:go_default_library",
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
)
