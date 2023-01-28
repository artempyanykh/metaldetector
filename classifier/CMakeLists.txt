cmake_minimum_required(VERSION 3.25)

# Setup VCPKG
set(VCPKG_ROOT "vcpkg")
set(CMAKE_TOOLCHAIN_FILE "${VCPKG_ROOT}/scripts/buildsystems/vcpkg.cmake" CACHE STRING "")

# Define the project
project(classifier)
set(CMAKE_CXX_STANDARD 20)

message(STATUS "CMAKE_HOST_SYSTEM_NAME = ${CMAKE_HOST_SYSTEM_NAME}")
message(STATUS "CMAKE_SYSTEM_NAME = ${CMAKE_SYSTEM_NAME}")
message(STATUS "CMAKE_CROSSCOMPILING = ${CMAKE_CROSSCOMPILING}")

add_executable(classifier main.cpp)
