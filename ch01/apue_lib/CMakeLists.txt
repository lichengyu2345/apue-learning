set(target_name "apue_lib")

add_library(${target_name} error.c errorlog.c)

target_include_directories(${target_name} INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})

