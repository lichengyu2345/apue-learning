cmake_minimum_required (VERSION 2.8)

project(apue)

add_subdirectory(apue_lib)

set(target_name "1.3")
list(APPEND my_srcs "1.3.c")
add_executable(${target_name} ${my_srcs})

target_include_directories(${target_name} PUBLIC apue_lib)
target_link_libraries(${target_name} apue_lib)
