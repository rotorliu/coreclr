cmake_minimum_required(VERSION 2.8.12.2)

project(PALTESTSUITE)

include_directories(${PALTESTSUITE_SOURCE_DIR}/common)

add_compile_options(-Wno-incompatible-pointer-types-discards-qualifiers)
add_compile_options(-Wno-int-to-void-pointer-cast)

# TODO: make these tests compile
# add_subdirectory(composite)
add_subdirectory(exception_handling)

add_subdirectory(c_runtime)
add_subdirectory(debug_api)
add_subdirectory(filemapping_memmgt)
add_subdirectory(file_io)
add_subdirectory(loader)
add_subdirectory(locale_info)
add_subdirectory(miscellaneous)
add_subdirectory(pal_specific)
add_subdirectory(samples)
add_subdirectory(threading)

