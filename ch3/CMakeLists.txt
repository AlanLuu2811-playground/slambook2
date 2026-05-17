cmake_minimum_required(VERSION 2.8)
project(chapter3)

set(CMAKE_CXX_FLAGS "-std=c++11")

# Add header file
include_directories("/usr/include/eigen3")

add_executable(eigenMatrix eigenMatrix.cpp)
add_executable(eigenGeometry useGeometry.cpp)
add_executable(coordinateTrans coordinateTransform.cpp)

add_subdirectory(examples)
add_subdirectory(visualizeGeometry)
