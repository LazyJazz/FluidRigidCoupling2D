cmake_minimum_required(VERSION 3.22)

set(CMAKE_TOOLCHAIN_FILE "${CMAKE_CURRENT_SOURCE_DIR}/vcpkg/scripts/buildsystems/vcpkg.cmake")

project(fluid-rigid-coupling)

set(CMAKE_CXX_STANDARD 17)

add_subdirectory(src)