cmake_minimum_required(VERSION 2.6 FATAL_ERROR)

project(narf_test)

find_package(PCL 1.3 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable (narf_test narf_test.cpp)
target_link_libraries (narf_test ${PCL_LIBRARIES})
