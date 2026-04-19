cmake_minimum_required(VERSION 3.31.10)
project(hello-world)
add_executable(${CMAKE_PROJECT_NAME})

if (${CMAKE_CXX_COMPILER} MATCHES "mingw")
    target_link_options(${CMAKE_PROJECT_NAME} PRIVATE --static)
endif()

add_subdirectory(src)