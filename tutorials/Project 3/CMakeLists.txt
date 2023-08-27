cmake_minimum_required(VERSION 3.26)
project(tutorial_03_pick_device)
add_executable(tutorial_03_pick_device main.cpp)

find_package(Vulkan REQUIRED)
find_package(glfw3 REQUIRED)
target_link_libraries(tutorial_03_pick_device Vulkan::Vulkan)
target_link_libraries(tutorial_03_pick_device glfw)