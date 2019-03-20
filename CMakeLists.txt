cmake_minimum_required(VERSION 3.12.2)

project(fun)

set(CMAKE_CXX_FLAGS "-g -Wall -std=c++17")

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

message(${SDL2_INCLUDE_DIRS})

add_executable(lession01 Lession01.cpp)
add_executable(lession02 Lession02.cpp)
target_link_libraries(lession01 ${SDL2_LIBRARIES})
target_link_libraries(lession02 ${SDL2_LIBRARIES})