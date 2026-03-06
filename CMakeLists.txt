cmake_minimum_required(VERSION 3.23)
project(hello-world)
add_executable(hello-world)
target_sources(hello-world
    PRIVATE
        main.cpp
)