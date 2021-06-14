cmake_minimum_required(VERSION 3.19)
project(DreamWorld)

set(CMAKE_CXX_STANDARD 20)
find_package(Vulkan REQUIRED)
find_package(glfw3 3.3.4 REQUIRED)

add_executable(DreamWorld main.cpp)

target_link_libraries(DreamWorld glfw)
target_link_libraries(DreamWorld Vulkan::Vulkan)

SET(VK_ICD_FILENAMES, /Users/achintya/VulkanSDK/1.2.176.1/macOS/share/vulkan/icd.d/MoltenVK_icd.json)
SET(VK_LAYER_PATH, /Users/achintya/VulkanSDK/1.2.176.1/macOS/share/vulkan/explicit_layer.d)


