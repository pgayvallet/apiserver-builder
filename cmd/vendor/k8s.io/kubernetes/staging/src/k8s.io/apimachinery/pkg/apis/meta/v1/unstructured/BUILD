package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["unstructured_test.go"],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apimachinery/pkg/apis/meta/v1/unstructured",
    library = ":go_default_library",
    tags = ["automanaged"],
)

go_library(
    name = "go_default_library",
    srcs = [
        "unstructured.go",
        "zz_generated.deepcopy.go",
    ],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/apimachinery/pkg/apis/meta/v1/unstructured",
    tags = ["automanaged"],
    deps = [
        "//cmd/vendor/github.com/golang/glog:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/conversion:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/conversion/unstructured:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/json:go_default_library",
        "//cmd/vendor/k8s.io/apimachinery/pkg/util/runtime:go_default_library",
    ],
)
