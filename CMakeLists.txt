cmake_minimum_required(VERSION 2.8)
project(slam_code_study)

#set(CMAKE_CXX_FLAGS "-fPIC")
set(CMAKE_BUILD_TYPE "Debug")
set(CMAKE_CXX_STANDARD 11)

add_subdirectory(src)
add_subdirectory(src_bin)

