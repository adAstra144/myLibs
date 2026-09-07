cmake_minimum_required(VERSION 3.15)
project(myTools LANGUAGES CXX)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_library(myTools STATIC
    src/devTools.cpp
)

target_include_directories(myTools PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)

target_compile_features(myTools PUBLIC cxx_std_17)