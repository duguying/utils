cmake_minimum_required(VERSION 2.8.4)
project(utils)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

include_directories("include")

set(
    UTILS_SOURCE_FILES
    src/ds.c
    src/file.c
    src/hashtable.c
    src/process.c
    src/sock.c
    src/stack.c
    src/thread.c
    )
add_library(base STATIC ${UTILS_SOURCE_FILES})
