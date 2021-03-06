package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = [
        "constants.go",
        "httpstream.go",
        "portforward.go",
        "websocket.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/kubelet/server/portforward",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/golang/glog:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/httpstream:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/httpstream/spdy:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/runtime:go_default_library",
        "//cmd/vendor/k8s.io/apiserver/pkg/server/httplog:go_default_library",
        "//cmd/vendor/k8s.io/apiserver/pkg/util/wsstream:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/api:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "httpstream_test.go",
        "websocket_test.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/kubelet/server/portforward",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/httpstream:go_default_library",
        "//cmd/vendor/k8s.io/kubernetes/pkg/api:go_default_library",
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
