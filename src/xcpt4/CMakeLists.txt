add_executable(xcpt4
    xcpt4cxx.cpp
    xcpt4ex.c
    xcpt4pg.c
    xcpt4u.c
)

target_compile_options(xcpt4 PRIVATE -fms-extensions -fno-inline -fasync-exceptions)
target_compile_definitions(xcpt4 PRIVATE BAIL_IN_FINALLY)
