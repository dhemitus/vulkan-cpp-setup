cmake_minimum_required(VERSION 3.0...4.0)
project(
  vulkan_setup
  VERSION 0.1.0
  LANGUAGES CXX C)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR})
set(CMAKE_CXX_STANDARD 20)

add_subdirectory(vendor)
add_subdirectory(src)
