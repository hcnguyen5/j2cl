load(
    "//transpiler/javatests/com/google/j2cl/integration:integration_test.bzl",
    "integration_test",
)

package(
    licenses = ["notice"],  # Apache 2.0
)

# Creates targets
# blaze build :optimized_js
# blaze test :readable_js
integration_test(
    name = "staticfieldcollision",
    srcs = glob(["*.java"]),
    enable_wasm = True,
    deps = ["//third_party:gwt-jsinterop-annotations-j2cl"],
)
