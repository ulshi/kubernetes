load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "errors.go",
        "microversions.go",
        "requests.go",
        "results.go",
        "urls.go",
        "util.go",
    ],
    importmap = "k8s.io/kubernetes/vendor/github.com/gophercloud/gophercloud/openstack/compute/v2/servers",
    importpath = "github.com/gophercloud/gophercloud/openstack/compute/v2/servers",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/gophercloud/gophercloud:go_default_library",
        "//vendor/github.com/gophercloud/gophercloud/openstack/compute/v2/flavors:go_default_library",
        "//vendor/github.com/gophercloud/gophercloud/openstack/compute/v2/images:go_default_library",
        "//vendor/github.com/gophercloud/gophercloud/pagination:go_default_library",
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
