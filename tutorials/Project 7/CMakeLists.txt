cmake_minimum_required(VERSION 3.26)
project(tutorial_02_07_image_view)
add_executable(tutorial_02_07_image_view main.cpp)

find_package(Vulkan REQUIRED)
find_package(glfw3 REQUIRED)
target_link_libraries(tutorial_02_07_image_view Vulkan::Vulkan)
target_link_libraries(tutorial_02_07_image_view glfw)