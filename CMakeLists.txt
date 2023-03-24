cmake_minimum_required(VERSION 3.16)
project(doctest LANGUAGES CXX VERSION 2.4.11)

### Targets

add_library(doctest STATIC ./source/doctest.cpp)
target_compile_features(doctest PUBLIC cxx_std_11)
target_compile_definitions(doctest PUBLIC DOCTEST_CONFIG_USE_STD_HEADERS)
target_include_directories(doctest PUBLIC ./include)
