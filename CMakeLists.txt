cmake_minimum_required(VERSION 2.8)

project(Learn_OpenGL)

add_subdirectory("C:/Users/Mehdi/Library sources/glfw-3.2.1" "glfw-3.2.1" EXCLUDE_FROM_ALL)
include_directories(
    "C:/Users/Mehdi/Library sources/glad/include"
)

add_executable(${PROJECT_NAME}
    "main.cpp"
    "glad.c"
)
target_link_libraries(${PROJECT_NAME}
    glfw
)
