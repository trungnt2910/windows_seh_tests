add_library(xframe_eh_dll SHARED
    xframe_eh_dll.c
    xframe_eh_dll.DEF
)

target_compile_options(xframe_eh_dll PRIVATE -fms-extensions)
