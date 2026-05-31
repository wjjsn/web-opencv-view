cmake_minimum_required(VERSION 3.15)
project(hello_world)

find_package(OpenCV REQUIRED)
find_package(CivetWeb REQUIRED)

add_executable(hello_world main.cpp)

target_link_libraries(hello_world PRIVATE
    opencv::opencv
    civetweb::civetweb-cpp
)

# Print version info
message(STATUS "OpenCV version: ${OpenCV_VERSION}")
message(STATUS "CivetWeb version: ${CivetWeb_VERSION}")
