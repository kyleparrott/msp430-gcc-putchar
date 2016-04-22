# putchar CMake build
cmake_minimum_required (VERSION 2.8)
project (putchar)

add_library (putchar STATIC
             Source/putchar.c)

target_sources (putchar PRIVATE Source/putchar.c)
target_include_directories (putchar PUBLIC ${CMAKE_CURRENT_LIST_DIR})
