cmake_minimum_required(VERSION 3.17)
project(cpp_simple_opengl)

set(CMAKE_CXX_STANDARD 14)

# Source files.
set(SOURCE_FILES
        main.cpp)

# Tell CMake to create the executable.
add_executable(cpp_simple_opengl ${SOURCE_FILES})
