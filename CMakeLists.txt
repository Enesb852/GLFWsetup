cmake_minimum_required(VERSION 3.14)
project(GLFWsetup)

add_subdirectory(deps/glfw)

find_package(OpenGL REQUIRED)

add_executable(GLFWSetup main.cpp)

target_link_libraries(GLFWSetup ${OPENGL_LIBRARIES} glfw)