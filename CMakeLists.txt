cmake_minimum_required(VERSION 2.8)
project( DisplayImage )

find_package( OpenCV REQUIRED )


include_directories( ${OpenCV_INCLUDE_DIRS} )

set (SOURCES
main.cpp
)

add_executable( main main.cpp ${SOURCES})

target_link_libraries( main ${OpenCV_LIBS} )