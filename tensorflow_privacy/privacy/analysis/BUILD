package(default_visibility = ["//visibility:public"])

licenses(["notice"])

py_library(
    name = "analysis",
    srcs = ["__init__.py"],
)

py_library(
    name = "compute_dp_sgd_privacy_lib",
    srcs = ["compute_dp_sgd_privacy_lib.py"],
)

py_binary(
    name = "compute_dp_sgd_privacy",
    srcs = ["compute_dp_sgd_privacy.py"],
    deps = [":compute_dp_sgd_privacy_lib"],
)

py_test(
    name = "compute_dp_sgd_privacy_test",
    size = "small",
    timeout = "moderate",
    srcs = ["compute_dp_sgd_privacy_test.py"],
    deps = [":compute_dp_sgd_privacy_lib"],
)

py_binary(
    name = "compute_noise_from_budget",
    srcs = ["compute_noise_from_budget.py"],
    deps = [":compute_noise_from_budget_lib"],
)

py_library(
    name = "compute_noise_from_budget_lib",
    srcs = ["compute_noise_from_budget_lib.py"],
)

py_test(
    name = "compute_noise_from_budget_test",
    srcs = ["compute_noise_from_budget_test.py"],
    deps = [":compute_noise_from_budget_lib"],
)

py_library(
    name = "gdp_accountant",
    srcs = ["gdp_accountant.py"],
)

py_library(
    name = "tensor_buffer",
    srcs = ["tensor_buffer.py"],
)

py_test(
    name = "tensor_buffer_eager_test",
    size = "small",
    srcs = ["tensor_buffer_eager_test.py"],
    deps = [":tensor_buffer"],
)

py_test(
    name = "tensor_buffer_graph_test",
    size = "small",
    srcs = ["tensor_buffer_graph_test.py"],
    deps = [":tensor_buffer"],
)

py_library(
    name = "tree_aggregation_accountant",
    srcs = ["tree_aggregation_accountant.py"],
)

py_test(
    name = "tree_aggregation_accountant_test",
    srcs = ["tree_aggregation_accountant_test.py"],
    deps = [":tree_aggregation_accountant"],
)
