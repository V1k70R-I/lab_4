cmake_minimum_required(VERSION 2.8)


project(my_project)

set(SOURCE_EXE main.c)

set(SOURCE_LIB add.c)

add_library(add STATIC ${SOURCE_LIB})

add_executable(main ${SOURCE_EXE})

target_link_libraries(main add)
