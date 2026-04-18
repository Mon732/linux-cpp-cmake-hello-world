cmake_minimum_required(VERSION 3.31.10)
project(hello-world)
add_executable(hello-world)

if (${CMAKE_CXX_COMPILER} MATCHES "mingw")
    target_link_options(hello-world PRIVATE --static)
endif()

add_subdirectory(src)