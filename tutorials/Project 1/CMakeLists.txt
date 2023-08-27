cmake_minimum_required(VERSION 3.26)
project(tutorial_01_hello_world)
add_executable(tutorial_01_hello_world main.cpp)

find_package(Vulkan REQUIRED)
find_package(glfw3 CONFIG REQUIRED)
target_link_libraries(tutorial_01_hello_world Vulkan::Vulkan)
target_link_libraries(tutorial_01_hello_world glfw)