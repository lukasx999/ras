cmake_minimum_required(VERSION 3.16)
set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)
set(CMAKE_EXPORT_COMPILE_COMMANDS TRUE)
set(CMAKE_COLOR_DIAGNOSTICS ON)

project(TDRF)

add_executable(tdrf main.cc Rasterizer.cc)
target_compile_options(tdrf PRIVATE -Wall -Wextra -O3 -ggdb)
target_link_libraries(tdrf raylib)
