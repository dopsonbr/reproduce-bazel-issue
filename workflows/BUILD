load("@io_bazel_rules_jsonnet//jsonnet:jsonnet.bzl", "jsonnet_library")

jsonnet_library(
    name = "workflow",
    srcs = ["martinis.libsonnet"],
)

jsonnet_to_json(
    name = "wordcount",
    src = "wordcount.jsonnet",
    outs = ["wordcount.json"],
    deps = [":workflow"],
)
