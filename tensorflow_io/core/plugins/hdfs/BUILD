licenses(["notice"])  # Apache 2.0

package(default_visibility = ["//visibility:public"])

load(
    "//:tools/build/tensorflow_io.bzl",
    "tf_io_copts",
)

cc_library(
    name = "hdfs",
    srcs = [
        "hadoop_filesystem.cc",
    ],
    copts = tf_io_copts(),
    linkstatic = True,
    deps = [
        "//tensorflow_io/core/plugins:plugins_header",
        "@hadoop",
    ],
    alwayslink = 1,
)
