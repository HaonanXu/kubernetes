load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["tasks.pb.go"],
    importmap = "k8s.io/kubernetes/vendor/github.com/containerd/containerd/api/services/tasks/v1",
    importpath = "github.com/containerd/containerd/api/services/tasks/v1",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/containerd/containerd/api/types:go_default_library",
        "//vendor/github.com/containerd/containerd/api/types/task:go_default_library",
        "//vendor/github.com/gogo/protobuf/proto:go_default_library",
        "//vendor/github.com/gogo/protobuf/types:go_default_library",
        "//vendor/github.com/opencontainers/go-digest:go_default_library",
        "//vendor/golang.org/x/net/context:go_default_library",
        "//vendor/google.golang.org/grpc:go_default_library",
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
