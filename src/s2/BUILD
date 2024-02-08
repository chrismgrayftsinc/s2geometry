load("@rules_cc//cc:defs.bzl", "cc_library", "cc_test")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "s2",
    srcs = glob(
        ["*.cc"],
        exclude = [
            "*_test.cc",
            "*testing.cc",
        ],
    ),
    hdrs = glob(["*.h"]),
    copts = ["-Isrc/"],
    deps = [
        "//src/s2/base:commandlineflags",
        "//src/s2/base:integral_types",
        "//src/s2/base:logging",
        "//src/s2/base:port",
        "//src/s2/base:spinlock",
        "//src/s2/testing",
        "//src/s2/util/bitmap",
        "//src/s2/util/bits",
        "//src/s2/util/coding",
        "//src/s2/util/endian",
        "//src/s2/util/gtl",
        "//src/s2/util/hash",
        "//src/s2/util/math:mathutil",
        "//src/s2/util/math:matrix3x3",
        "//src/s2/util/math:vector",
        "//src/s2/util/math/exactfloat",
        "//src/s2/util/units",
        "@com_google_absl//absl/base",
        "@com_google_absl//absl/flags:flag",
        "@com_google_absl//absl/log:absl_log",
        "@com_google_absl//absl/log:check",
        "@com_google_absl//absl/status",
    ],
)

cc_test(
    name = "s2shapeutil_count_edges_test",
    srcs = [
        "s2shapeutil_count_edges_test.cc",
    ],
    copts = ["-Isrc/"],
    deps = [
        ":s2",
        "@com_google_googletest//:gtest_main",
    ],
)
