cmake_minimum_required(VERSION 3.23)
project(2D_Renderer)

set(CMAKE_CXX_STANDARD 23)

add_subdirectory(dependencies/glad)
add_subdirectory(dependencies/glfw)

add_executable(2D_Renderer src/main.cpp)

target_link_libraries(2D_Renderer PUBLIC glfw glad)