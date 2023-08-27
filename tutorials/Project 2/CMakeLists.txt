cmake_minimum_required(VERSION 3.26)
project(tutorial_02_validation_layers)

set(CMAKE_CXX_STANDARD 17)

add_executable(tutorial_02_validation_layers main.cpp)

find_package(Vulkan REQUIRED)
find_package(glfw3 REQUIRED)
target_link_libraries(tutorial_02_validation_layers Vulkan::Vulkan)
target_link_libraries(tutorial_02_validation_layers glfw)