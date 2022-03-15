load("@io_bazel_rules_scala//scala:scala.bzl", "scala_library", "scala_binary", "scala_test")

# stage 2

scala_binary(
    name = "ProjectRunner",
    srcs = ["src/main/scala/com/example/ProjectRunner.scala"],
    main_class = "com.example.ProjectRunner",
    deps = [":greeter"],
)

scala_library(
    name = "greeter",
    srcs = ["src/main/scala/com/example/Greeting.scala"],
)


# without java installed need to use:
# --java_runtime_version=remotejdk_11
# ... or equivalent

# also seem to require
# --incompatible_java_common_parameters=false