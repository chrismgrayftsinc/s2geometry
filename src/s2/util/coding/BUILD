load("@rules_cc//cc:defs.bzl", "cc_library")
package(default_visibility = ["//visibility:public"])

cc_library(
    name = "coding",
    copts = ["-Isrc/"],
    srcs = [
        "coder.cc",
        "varint.cc",
    ],
    hdrs = [
        "coder.h",
        "varint.h",
        "nth-derivative.h",
        "transforms.h",
    ],
    deps = [
        "//src/s2/base:integral_types",
        "//src/s2/base:casts",
        "//src/s2/base:logging",
        "//src/s2/base:port",
        "//src/s2/util/bits",
        "//src/s2/util/endian",
        "@absl//absl/base",
        "@absl//absl/strings:cord",
        "@absl//absl/container:btree",
        "@absl//absl/container:flat_hash_set",
    ],
)
