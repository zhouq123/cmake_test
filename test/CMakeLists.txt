cmake_minimum_required(VERSION 2.8)

project(hello_test)

# Enable C++11
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)

# Add the application sources to the target
add_executable(${PROJECT_NAME} hello_test.cpp)

target_link_libraries(${PROJECT_NAME})