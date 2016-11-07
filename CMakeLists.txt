cmake_minimum_required(VERSION 3.6)
project(lmp)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

file(GLOB_RECURSE SRCS ${PROJECT_SOURCE_DIR}/src/*.cpp)
include_directories(include)

add_library(${PROJECT_NAME} SHARED ${SRCS})
