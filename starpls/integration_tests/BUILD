load("//:starpls.bzl", "setup_starpls")
load(":defs.bzl", "starpls_py_integration_test")

setup_starpls(
    name = "_starpls_binary_for_test",
    visibility = ["//starpls/integration_tests:__pkg__"],
)

starpls_py_integration_test(
    name = "starpls_test",
    srcs = ["starpls_test.py"],
    data = [":_starpls_binary_for_test_bin"],
)