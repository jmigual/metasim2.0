cmake_minimum_required (VERSION 3.1)
project (metasim)

if(NOT CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE Release)
endif()
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall") 
set(CMAKE_CXX_STANDARD 14) 

set(LIBRARY_TYPE STATIC)

# Include dirs.
add_subdirectory (src)
add_subdirectory (examples)

enable_testing (true)
add_subdirectory (test)
