load("@rules_cc//cc:defs.bzl", "cc_library")
package(default_visibility = ["//visibility:public"])

cc_library(
    name = "vector",
    hdrs = ["vector.h"],
)

cc_library(
    name = "mathutil",
    copts = ["-Isrc/"],
    srcs = ["mathutil.cc"],
    hdrs = ["mathutil.h"],
    deps = [
        "//src/s2/base:integral_types",
        "//src/s2/base:logging",
        "//src/s2/util/bits",
        "@absl//absl/log",
        "@absl//absl/log:check",
    ],
)

cc_library(
    name = "matrix3x3",
    hdrs = ["matrix3x3.h"],
)
