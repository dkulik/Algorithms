# the usual boilerplate setup
cmake_minimum_required(VERSION 3.1)
project(tests LANGUAGES CXX)

# tell CMake to use CTest extension
enable_testing()

# create an executables for each algorithm
add_executable(test1 test1.cxx)
add_executable(test2 test2.cxx)

# register test CTest
add_test(NAME TEST1_OK_EXPECTED COMMAND test1)
add_test(NAME TEST2_FAIL_EXPECTED COMMAND test2)

