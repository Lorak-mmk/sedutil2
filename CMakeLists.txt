cmake_minimum_required(VERSION 3.18)
project(sedutil2)

set(CMAKE_CXX_STANDARD 14)

add_executable(sedutil2-cli)
# IT needs to be here insted of src/Common/version/commithash.cmake because of cmake bug: https://gitlab.kitware.com/cmake/cmake/-/issues/18399
set_source_files_properties(
        ${CMAKE_CURRENT_BINARY_DIR}/src/Common/version/commithash.c
        PROPERTIES GENERATED TRUE
)

add_subdirectory(src)



