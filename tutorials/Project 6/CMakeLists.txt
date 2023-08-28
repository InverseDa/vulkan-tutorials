cmake_minimum_required(VERSION 3.26)
project(tutorial_02_06_swap_chain)
add_executable(tutorial_02_06_swap_chain main.cpp)

find_package(Vulkan REQUIRED)
find_package(glfw3 REQUIRED)
target_link_libraries(tutorial_02_06_swap_chain Vulkan::Vulkan)
target_link_libraries(tutorial_02_06_swap_chain glfw)