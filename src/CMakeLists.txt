add_subdirectory(Common)

if(UNIX AND NOT APPLE)
    add_subdirectory(linux)
elseif(WIN32)
    add_subdirectory(windows)
else()
    message( FATAL_ERROR "Your os is not supported." )
endif()
