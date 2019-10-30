cmake_minimum_required(VERSION 2.8)
project(slam_code_study)

set(CMAKE_BUILD_TYPE "Debug")
set(CMAKE_CXX_STANDARD 11)

#include_directories(../include)

set(HEADERS 
            ${PROJECT_SOURCE_DIR}/../include/libHelloSLAM.h
   )
set(SOURCES_FILES
            libHelloSLAM.cpp 
   )
set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/../lib )

add_library(helloSLAM_shared SHARED ${HEADERS} ${SOURCES_FILES})
