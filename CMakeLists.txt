cmake_minimum_required(VERSION 3.17)
project(foo LANGUAGES C)
add_library(foo)
target_sources(foo
    PUBLIC foo.h
    PRIVATE foo.c
)
target_include_directories(foo
    PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}
)
