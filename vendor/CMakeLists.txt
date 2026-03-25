add_subdirectory(GLFW)
add_subdirectory(glm)
add_subdirectory(tinyobjloader)
find_package(Vulkan REQUIRED)

add_library(vendor INTERFACE)
target_link_libraries(vendor INTERFACE tinyobjloader glm glfw Vulkan::Vulkan)
