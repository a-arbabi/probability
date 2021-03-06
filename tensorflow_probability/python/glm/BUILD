# Copyright 2018 The TensorFlow Probability Authors.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
# ============================================================================
# Description:
#   Generalized Linear Model specification, fitting, and related utilities.

package(
    default_visibility = [
        "//tensorflow_probability:__subpackages__",
    ],
)

licenses(["notice"])  # Apache 2.0

exports_files(["LICENSE"])

py_library(
    name = "glm",
    srcs = ["__init__.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":family",
        ":fisher_scoring",
    ],
)

py_library(
    name = "fisher_scoring",
    srcs = ["fisher_scoring.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":util",
        # numpy dep,
        # tensorflow dep,
    ],
)

py_test(
    name = "fisher_scoring_test",
    size = "small",
    srcs = ["fisher_scoring_test.py"],
    deps = [
        # numpy dep,
        # tensorflow dep,
        "//tensorflow_probability",
    ],
)

py_library(
    name = "family",
    srcs = ["family.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":util",
        # numpy dep,
        # tensorflow dep,
    ],
)

py_test(
    name = "family_test",
    size = "small",
    srcs = ["family_test.py"],
    deps = [
        # numpy dep,
        # tensorflow dep,
        "//tensorflow_probability",
    ],
)

py_library(
    name = "util",
    srcs = ["util.py"],
    srcs_version = "PY2AND3",
    deps = [
        # numpy dep,
        # tensorflow dep,
    ],
)
