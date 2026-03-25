add_executable(${PROJECT_NAME})

target_sources(${PROJECT_NAME} PRIVATE main.cpp)
set_target_properties(
  ${PROJECT_NAME}
  PROPERTIES CXX_STANDARD 20
             CXX_STANDARD_REQUIRED ON
             CXX_EXTENSIONS OFF
             COMPILE_WARNING_AS_ERROR ON
             CMAKE_EXPORT_COMPILE_COMMANDS ON)

target_compile_options(${PROJECT_NAME} PRIVATE -Wall)
target_link_libraries(${PROJECT_NAME} PRIVATE vendor)

target_include_directories(${PROJECT_NAME} PRIVATE vendor)
