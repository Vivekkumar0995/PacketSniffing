cmake_minimum_required(VERSION 4.2)
project(packetsniff LANGUAGES C CXX)

include(FetchContent)
find_package(PkgConfig REQUIRED)
add_executable(packetsn main.cpp src/some.cpp)

target_include_directories(packetsn PRIVATE headers)
