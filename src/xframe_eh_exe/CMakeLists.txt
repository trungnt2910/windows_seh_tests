add_executable(xframe_eh_exe xframe_eh_exe.c)

target_compile_options(xframe_eh_exe PRIVATE -fms-extensions)

# Ensure the DLL is built before the executable so it is available at runtime
add_dependencies(xframe_eh_exe xframe_eh_dll)
