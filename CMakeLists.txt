cmake_minimum_required(VERSION 3.10)
project(LearnOpenGL)

include_directories(${CMAKE_SOURCE_DIR}/include)

add_executable(myprogram main.cpp glad.c shader.cpp camera.cpp stb_image.cpp)

target_link_libraries(myprogram ${CMAKE_SOURCE_DIR}/libs/GLFW/libglfw3.a GL X11 pthread Xrandr Xi dl)
