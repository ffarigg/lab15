cmake_minimum_required(VERSION 3.26)
project(lab15 C)

set(CMAKE_C_STANDARD 11)

add_executable(lab15 main.c
        libs/data_structers/matrix/matrix.c
        libs/data_structers/matrix/matrix.h)

add_subdirectory(libs)
target_link_libraries(lab15 data_structures)