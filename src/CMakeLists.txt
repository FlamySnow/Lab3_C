cmake_minimum_required(VERSION 3.20)
project(Lab3_C)

set(CMAKE_CXX_STANDARD 20)

add_executable(Lab3_C main.cpp)

find_library(LIB_PATH PCB
        PATHS
        ../lib/cmake-build-debug/)

target_include_directories(Lab3_C PRIVATE ../lib)

TARGET_LINK_LIBRARIES( Lab3_C ${LIB_PATH} )
