cmake_minimum_required(VERSION 2.8)
project( image_abstraction )
find_package( OpenCV REQUIRED )
include_directories( lime/sources )
add_executable( image_abstraction image_abstraction.cpp )
target_link_libraries( image_abstraction ${OpenCV_LIBS} )
SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++14") 
