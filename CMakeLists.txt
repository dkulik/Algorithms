cmake_minimum_required(VERSION 3.0.0)

project(Algorithms VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 17)

include(CTest)

enable_testing()

set_property(GLOBAL PROPERTY CTEST_TARGETS_ADDED 1)

# set binaries output path 
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_SOURCE_DIR}/bin")

# Include source code and headers.
add_subdirectory(source)

