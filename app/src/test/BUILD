load("@rules_jvm_external//:defs.bzl", "artifact")
load("@io_bazel_rules_kotlin//kotlin:kotlin.bzl", "kt_android_local_test")

package(default_visibility = ["//visibility:public"])

kt_android_local_test(
    name = "bitrise_test",
    custom_package = "io.bitrise.sample.android",
    srcs = glob(["java/io/bitrise/sample/android/ExampleUnitTest.kt"]),
    manifest = "AndroidManifest.xml",
    test_class = "io.bitrise.sample.android.ExampleUnitTest",
    deps = [
        artifact("junit:junit"),
        "@robolectric//bazel:android-all"
    ],
)