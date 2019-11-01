cmake_minimum_required(VERSION 3.10)
project(doctest LANGUAGES CXX VERSION 2.3.5)

add_library(doctest STATIC ./source/doctest.cpp)
target_compile_features(doctest PUBLIC cxx_std_11)
target_include_directories(doctest PUBLIC ./include)
