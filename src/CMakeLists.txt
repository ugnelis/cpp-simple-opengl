cmake_minimum_required(VERSION 3.17)
project(cpp_simple_opengl)

set(CMAKE_CXX_STANDARD 14)

# Find the OpenGL libraries.
find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)

# Libraries.
set(LIBS
        ${OPENGL_LIBRARY}
        ${GLUT_LIBRARY})

# Source files.
set(SOURCE_FILES
        main.cpp)

# Tell CMake to create the executable.
add_executable(${PROJECT_NAME} ${SOURCE_FILES})

# Link libraries with project.
target_link_libraries(${PROJECT_NAME} ${LIBS})
