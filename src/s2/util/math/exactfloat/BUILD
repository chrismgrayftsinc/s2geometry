load("@rules_cc//cc:defs.bzl", "cc_library")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "exactfloat",
    srcs = ["exactfloat.cc"],
    hdrs = ["exactfloat.h"],
    copts = ["-Isrc/"],
    deps = [
        "//src/s2/base:integral_types",
        "//src/s2/base:logging",
        "//src/s2/base:port",
        "@boringssl//:crypto",
        "@com_google_absl//absl/log",
    ],
)
