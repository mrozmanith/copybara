# Copyright 2016 Google Inc.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.


licenses(["notice"])  # Apache 2.0

sh_test(
    name = "tool_test",
    srcs = ["tool_test.sh"],
    data = [
        "//java/com/google/copybara",
        "//third_party/bazel/bashunit",
    ],
    tags = ["local"],
    visibility = ["//visibility:public"],
)

py_binary(
    name = "cram",
    srcs = ["cram.py"],
    deps = ["@cram//:cramlib"],
)

load("//copybara/integration:cram.bzl", "cram_test")

#cram_test(
#    name = "hello",
#    srcs = ["hello.t"],
#)

#cram_test(
#    name = "test-preserve-env.t",
#    srcs = ["test-preserve-env.t"],
#    deps = ["//java/com/google/copybara"],
#)

#cram_test(
#    name = "test-help.t",
#    srcs = ["test-help.t"],
#    deps = ["//java/com/google/copybara"],
#)
