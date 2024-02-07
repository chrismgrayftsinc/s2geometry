load("@rules_cc//cc:defs.bzl", "cc_library")
package(default_visibility = ["//visibility:public"])

cc_library(
    name = "logging",
    hdrs = [
        "logging.h",
        "log_severity.h",
    ],
    deps = [
        "@absl//absl/log:absl_log",
        "@absl//absl/log:check",
    ],
)

cc_library(
    name = "integral_types",
    hdrs = ["integral_types.h"],
)

cc_library(
    name = "casts",
    hdrs = ["casts.h"],
    deps = [
        "@absl//absl/log",
    ],
)

cc_library(
    name = "port",
    hdrs = ["port.h"],
)

cc_library(
    name = "commandlineflags",
    hdrs = [
        "commandlineflags.h",
        "commandlineflags_declare.h",
    ],
)

cc_library(
    name = "spinlock",
    hdrs = [
        "spinlock.h",
    ],
)
