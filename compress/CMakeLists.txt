
include_directories(${REACTOS_SOURCE_DIR}/sdk/lib/conutils)

add_executable(compress mscompress.c mscompress.rc)
set_module_type(compress win32cui UNICODE)
target_link_libraries(compress conutils ${PSEH_LIB})
add_importlibs(compress msvcrt kernel32)
add_cd_file(TARGET compress DESTINATION reactos/system32 FOR all)
