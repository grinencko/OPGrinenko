cmake_minimum_required(VERSION 3.23)
project(gitgrinencko C)

set(CMAKE_C_STANDARD 11)

add_executable(gitgrinencko main.c libs/algorithms/array/array.c libs/algorithms/array/array.h libs/algorithms/algorithm.c)

add_subdirectory(libs)
target_link_libraries(gitgrinencko data_structures)
target_link_libraries(gitgrinencko algorithms)