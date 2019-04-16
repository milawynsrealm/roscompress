
include_directories(${REACTOS_SOURCE_DIR}/sdk/lib/conutils)

add_executable(expand msexpand.c msexpand.rc)
set_module_type(expand win32cui UNICODE)
target_link_libraries(expand conutils ${PSEH_LIB})
add_importlibs(expand msvcrt kernel32)
add_cd_file(TARGET expand DESTINATION reactos/system32 FOR all)
