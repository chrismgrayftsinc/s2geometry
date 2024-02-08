load("@rules_cc//cc:defs.bzl", "cc_library")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "coding",
    srcs = [
        "coder.cc",
        "varint.cc",
    ],
    hdrs = [
        "coder.h",
        "nth-derivative.h",
        "transforms.h",
        "varint.h",
    ],
    copts = ["-Isrc/"],
    deps = [
        "//src/s2/base:casts",
        "//src/s2/base:integral_types",
        "//src/s2/base:logging",
        "//src/s2/base:port",
        "//src/s2/util/bits",
        "//src/s2/util/endian",
        "@com_google_absl//absl/base",
        "@com_google_absl//absl/container:btree",
        "@com_google_absl//absl/container:flat_hash_set",
        "@com_google_absl//absl/strings:cord",
    ],
)
