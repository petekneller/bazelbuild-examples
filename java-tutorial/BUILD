load("@rules_java//java:defs.bzl", "java_binary", "java_library")

# stage 1

# java_binary(
#     name = "ProjectRunner",
#     srcs = glob(["src/main/java/com/example/*.java"]),
# )

# stage 2

java_binary(
    name = "ProjectRunner",
    srcs = ["src/main/java/com/example/ProjectRunner.java"],
    main_class = "com.example.ProjectRunner",
    deps = [":greeter"],
)

java_library(
    name = "greeter",
    srcs = ["src/main/java/com/example/Greeting.java"],
    visibility = ["//src/main/java/com/example/cmdline:__pkg__"],
)


# without java installed need to use:
# --java_runtime_version=remotejdk_11
# ... or equivalent