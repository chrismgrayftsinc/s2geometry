load("@rules_cc//cc:defs.bzl", "cc_library")
package(default_visibility = ["//visibility:public"])

cc_library(
    name = "exactfloat",
    copts = ["-Isrc/"],
    srcs = ["exactfloat.cc"],
    hdrs = ["exactfloat.h"],
    deps = [
        "//src/s2/base:integral_types",
        "//src/s2/base:logging",
        "//src/s2/base:port",
        "@absl//absl/log",
        "@boringssl//:crypto",
    ],
)
