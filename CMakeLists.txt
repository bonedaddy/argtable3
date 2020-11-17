file(GLOB_RECURSE ARGTABLE_SOURCES
    ./deps/argtable3/*.h
    ./deps/argtable3/*.c
)

add_library(libargtable
    SHARED
        ${ARGTABLE_SOURCES}
)

target_compile_options(libargtable PRIVATE ${flags})
