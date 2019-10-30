cmake_minimum_required(VERSION 2.8)
project(slam_code_study)

set(CMAKE_BUILD_TYPE "Debug")
set(CMAKE_CXX_STANDARD 11)
#include_directories(../include)


set(EXECUTABLE_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/bin)

add_executable(helloSLAM useHello.cpp)

#target_link_libraries(helloSLAM ${PROJECT_SOURCE_DIR}/lib/helloSLAM_shared)
target_link_libraries(helloSLAM ${PROJECT_SOURCE_DIR}/../lib/helloSLAM_shared)