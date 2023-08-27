cmake_minimum_required(VERSION 3.26)
project(tutorial_03)

set(CMAKE_CXX_STANDARD 17)

add_executable(tutorial_03 main.cpp)

find_package(Vulkan REQUIRED)
find_package(glfw3 REQUIRED)
target_link_libraries(tutorial_03 Vulkan::Vulkan)
target_link_libraries(tutorial_03 glfw)