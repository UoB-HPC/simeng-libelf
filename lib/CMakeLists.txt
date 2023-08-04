set(LIB_SRCS 
    xasprintf.c
    xstrdup.c
    xstrndup.c
    xmalloc.c 
    next_prime.c
	crc32.c
    crc32_file.c
	color.c 
    error.c 
    printversion.c
)

add_library(elf-dep STATIC ${LIB_SRCS})

target_compile_definitions(elf-dep PUBLIC HAVE_ERROR_H HAVE_CONFIG_H)
target_include_directories(elf-dep PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
target_include_directories(elf-dep PRIVATE ${LIBELF_SRC})


