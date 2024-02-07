load("@rules_cc//cc:defs.bzl", "cc_library")
package(default_visibility = ["//visibility:public"])

cc_library(
    name = "s2",
    srcs = glob(["*.cc"], exclude = ["*_test.cc", "*testing.cc"]),
    hdrs = glob(["*.h"]),
    copts = ["-Isrc/"],
    deps = [
        "//src/s2/base:logging",
        "//src/s2/base:integral_types",
        "//src/s2/base:port",
        "//src/s2/base:commandlineflags",
        "//src/s2/base:spinlock",
        "//src/s2/util/coding",
        "//src/s2/util/gtl",
        "//src/s2/testing",
        "//src/s2/util/bits",
        "//src/s2/util/bitmap",
        "//src/s2/util/endian",
        "//src/s2/util/hash",
        "//src/s2/util/units",
        "//src/s2/util/math/exactfloat",
        "//src/s2/util/math:vector",
        "//src/s2/util/math:mathutil",
        "//src/s2/util/math:matrix3x3",
        "@absl//absl/base",
        "@absl//absl/status",
        "@absl//absl/log:check",
        "@absl//absl/log:absl_log",
        "@absl//absl/flags:flag",
    ],
)

