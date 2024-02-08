load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")
load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

git_repository(
    name = "boringssl",
    branch = "master-with-bazel",
    remote = "https://github.com/google/boringssl.git",
)

http_archive(
    name = "com_google_absl",
    urls = [
        "https://github.com/abseil/abseil-cpp/releases/download/20240116.0/abseil-cpp-20240116.0.tar.gz",
    ],
    strip_prefix = "abseil-cpp-20240116.0",
    sha256 = "338420448b140f0dfd1a1ea3c3ce71b3bc172071f24f4d9a57d59b45037da440",
)

# Bazel Skylib.
http_archive(
  name = "bazel_skylib",
  sha256 = "cd55a062e763b9349921f0f5db8c3933288dc8ba4f76dd9416aac68acee3cb94",
  urls = ["https://github.com/bazelbuild/bazel-skylib/releases/download/1.5.0/bazel-skylib-1.5.0.tar.gz"],
)

http_archive(
    name = "com_google_googletest",
    sha256 = "8ad598c73ad796e0d8280b082cebd82a630d73e73cd3c70057938a6501bba5d7",
    urls = ["https://github.com/google/googletest/archive/refs/tags/v1.14.0.tar.gz"],
    strip_prefix = "googletest-1.14.0",
)

load("@com_google_googletest//:googletest_deps.bzl", "googletest_deps")
googletest_deps()

# http_archive(
#     name = "glog",
#     urls = [
#         "https://github.com/google/glog/archive/refs/tags/v0.6.0.tar.gz",
#     ],
#     strip_prefix = "glob-0.6.0",
#     sha256 = "8a83bf982f37bb70825df71a9709fa90ea9f4447fb3c099e1d720a439d88bad6",
# )

# http_archive(
#     name = "com_github_gflags_gflags",
#     urls = [
#         "https://github.com/gflags/gflags/archive/refs/tags/v2.2.2.tar.gz",
#     ],
#     strip_prefix = "gflags-2.2.2",
#     sha256 = "34af2f15cf7367513b352bdcd2493ab14ce43692d2dcd9dfc499492966c64dcf",
# )
