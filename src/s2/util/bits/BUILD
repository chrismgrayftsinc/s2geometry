load("@rules_cc//cc:defs.bzl", "cc_library")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "bits",
    srcs = ["bit-interleave.cc"],
    hdrs = glob(["*.h"]),
    copts = ["-Isrc/"],
    deps = [
        "//src/s2/base:integral_types",
    ],
)
