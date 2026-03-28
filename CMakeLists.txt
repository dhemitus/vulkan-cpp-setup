cmake_minimum_required(VERSION 3.0...4.0)
project(
  vulkan_setup
  VERSION 0.1.0
  LANGUAGES CXX C)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR})
set(CMAKE_CXX_STANDARD 20)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
add_subdirectory(src)
target_include_directories(${PROJECT_NAME} PRIVATE vendor)
add_subdirectory(vendor)
