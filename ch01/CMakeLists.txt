cmake_minimum_required (VERSION 2.8)

project(apue)

add_subdirectory(apue_lib)

add_executable(apue 1.3.c)

target_include_directories(apue PUBLIC apue_lib)
target_link_libraries(apue apue_lib)
