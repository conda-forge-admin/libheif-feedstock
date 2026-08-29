cmake_minimum_required(VERSION 3.15)
project(test_libheif LANGUAGES CXX)

find_package(libheif CONFIG REQUIRED)

add_executable(test_libheif test.cpp)
target_link_libraries(test_libheif PRIVATE heif)
