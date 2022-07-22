cmake_minimum_required(VERSION 3.21)
project(MultiStorage)

set(CMAKE_CXX_STANDARD 20)

set(CMAKE_EXE_LINKER_FLAGS "-static")

find_package(Boost REQUIRED)
include_directories(${Boost_INCLUDE_DIR})

add_executable(MultiStorage main.cpp)
