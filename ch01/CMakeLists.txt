cmake_minimum_required (VERSION 3.14)

project(apue)

add_subdirectory(apue_lib)

set(target_name "1.4")
list(APPEND my_srcs "1.4.c")
add_executable(${target_name} ${my_srcs})

target_link_libraries(${target_name} PUBLIC apue_lib)
