cmake_minimum_required(VERSION 3.10)
project(doctest LANGUAGES CXX VERSION 1.2.7)

add_library(doctest INTERFACE)
target_include_directories(doctest INTERFACE ./doctest)
