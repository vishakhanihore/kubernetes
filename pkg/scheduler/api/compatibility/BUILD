load("@io_bazel_rules_go//go:def.bzl", "go_test")

go_test(
    name = "go_default_test",
    srcs = ["compatibility_test.go"],
    deps = [
        "//pkg/apis/core/install:go_default_library",
        "//pkg/scheduler:go_default_library",
        "//pkg/scheduler/algorithmprovider/defaults:go_default_library",
        "//pkg/scheduler/api:go_default_library",
        "//pkg/scheduler/apis/config:go_default_library",
        "//pkg/scheduler/core:go_default_library",
        "//pkg/scheduler/factory:go_default_library",
        "//staging/src/k8s.io/api/core/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//staging/src/k8s.io/client-go/informers:go_default_library",
        "//staging/src/k8s.io/client-go/kubernetes/fake:go_default_library",
        "//vendor/github.com/google/go-cmp/cmp:go_default_library",
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
