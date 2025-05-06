cmake_minimum_required(VERSION 3.12)

project(
    shared_futex
    VERSION 0.0.0
    LANGUAGES CXX
    DESCRIPTION "Fast, shared, upgradeable, non-recursive and non-fair mutex"
)

add_library(shared_futex INTERFACE)
target_include_directories(shared_futex INTERFACE include)
target_compile_features(shared_futex INTERFACE cxx_std_20)
set_target_properties(shared_futex PROPERTIES CXX_EXTENSIONS OFF)
