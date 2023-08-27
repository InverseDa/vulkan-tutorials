cmake_minimum_required(VERSION 3.26)
set(CMAKE_CXX_STANDARD 17)
project(vulkan_tutorials)
# 扫描子目录
file(GLOB tutorial_dirs "${CMAKE_CURRENT_SOURCE_DIR}/tutorials/Project *")
# 添加每个子目录
foreach(tutorial_dir ${tutorial_dirs})
    get_filename_component(tutorial_name ${tutorial_dir} NAME)
    add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/tutorials/${tutorial_name})
endforeach()