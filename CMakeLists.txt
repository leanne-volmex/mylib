cmake_minimum_required(VERSION 3.10)

# Set the project name
project(mylib)

# Set the output directory for the build artifacts
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)

# Add a library target called "my_library"
add_library(mylib STATIC src/mylib.cpp)

# Set the include directory for the library
target_include_directories(mylib PUBLIC include)
