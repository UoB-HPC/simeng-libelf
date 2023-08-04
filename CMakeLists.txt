cmake_minimum_required(VERSION 3.13)
project(simeng-libelf)

add_compile_options(-Wall -O2)

set(LIB_DEP_SRC ${CMAKE_CURRENT_SOURCE_DIR}/lib)
set(LIBELF_SRC ${CMAKE_CURRENT_SOURCE_DIR}/libelf)

add_subdirectory(lib)
add_subdirectory(libelf)


