workspace(name = "com_github_bazelbuild_buildifier")

http_archive(
    name = "io_bazel_rules_go",
    sha256 = "890e055a9956daa85287ed309e8efaa9d5336b2bc5a71ad3676c220c99015a9d",
    strip_prefix = "rules_go-0.3.2",
    url = "https://github.com/bazelbuild/rules_go/archive/0.3.2.tar.gz",
)

load("@io_bazel_rules_go//go:def.bzl", "go_repositories", "new_go_repository")
load("@io_bazel_rules_go//proto:go_proto_library.bzl", "go_proto_repositories")

go_repositories()

go_proto_repositories()

# used for build.proto
http_archive(
    name = "io_bazel",
    sha256 = "8e4646898fa9298422e69767752680d34cbf21bcae01c401b11aa74fcdb0ef66",
    strip_prefix = "bazel-0.4.1",
    url = "https://github.com/bazelbuild/bazel/archive/0.4.1.tar.gz",
)

new_go_repository(
    name = "org_golang_x_tools",
    commit = "3d92dd60033c312e3ae7cac319c792271cf67e37",
    importpath = "golang.org/x/tools",
)
