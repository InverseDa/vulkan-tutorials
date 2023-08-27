cmake_minimum_required(VERSION 3.26)
project(tutorial_04)

set(CMAKE_CXX_STANDARD 17)

add_executable(tutorial_04 main.cpp)

find_package(Vulkan REQUIRED)
find_package(glfw3 REQUIRED)
target_link_libraries(tutorial_04 Vulkan::Vulkan)
target_link_libraries(tutorial_04 glfw)