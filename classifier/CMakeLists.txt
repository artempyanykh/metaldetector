cmake_minimum_required(VERSION 3.25)

# Setup VCPKG
set(VCPKG_ROOT "vcpkg")
set(CMAKE_TOOLCHAIN_FILE "${VCPKG_ROOT}/scripts/buildsystems/vcpkg.cmake" CACHE STRING "")

# Define the project
project(classifier)
set(CMAKE_CXX_STANDARD 20)

add_executable(classifier main.cpp)
