set(CMAKE_INCLUDE_CURRENT_DIR ON)

include(commithash.cmake)

message("current binary dir: " ${CMAKE_CURRENT_BINARY_DIR})
message("binary dir: " ${CMAKE_BINARY_DIR})

target_sources(sedutil2-cli
        PRIVATE
            commithash.h
            ${CMAKE_CURRENT_BINARY_DIR}/commithash.c
)


target_include_directories(sedutil2-cli PRIVATE .)

# Add the dependency to the commithash target so it always gets run before being linked
add_dependencies(
    sedutil2-cli
    commithash
)
