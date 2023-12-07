# cmake_minimum_required(VERSION 3.14)
# project(my_project)

# # GoogleTest requires at least C++14
# set(CMAKE_CXX_STANDARD 14)
# set(CMAKE_CXX_STANDARD_REQUIRED ON)

# include(FetchContent)
# FetchContent_Declare(
#   googletest
#   URL https://github.com/google/googletest/archive/03597a01ee50ed33e9dfd640b249b4be3799d395.zip
# )
# # For Windows: Prevent overriding the parent project's compiler/linker settings
# set(gtest_force_shared_crt ON CACHE BOOL "" FORCE)
# FetchContent_MakeAvailable(googletest)

# enable_testing()

# add_executable(
#   hello_test
#   hello_test.cc
# )
# target_link_libraries(
#   hello_test
#   GTest::gtest_main
# )

# include(GoogleTest)
# gtest_discover_tests(hello_test)

# CMakeLists.txt

cmake_minimum_required(VERSION 3.12)
# Set the project name and version
project(MyProject)
set (CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_COMPILER "C:\\msys64\\ucrt64\\bin\\gcc.exe")
set(CMAKE_C_COMPILER "C:\\msys64\\ucrt64\\bin\\gcc.exe")


# Add the executable
add_executable(MyProject main.cpp)
