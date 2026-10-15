cmake_minimum_required(VERSION 3.10)
project(cmake_practice)

add_library(math_utils STATIC math_utils.cpp)

add_executable(app main.cpp)
target_link_libraries(app PRIVATE math_utils)