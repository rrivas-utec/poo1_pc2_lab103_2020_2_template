cmake_minimum_required(VERSION 3.10.2)
project(pc2)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/${OUTPUT_DEBUG})

add_executable(pc2
        main.cpp
        test_1.cpp
        test_2.cpp
        test_3.cpp
        p1.cpp p1.h
        p2.cpp p2.h
        p3.cpp p3.h
        )

configure_file(test_1.in ${CMAKE_RUNTIME_OUTPUT_DIRECTORY} COPYONLY)
configure_file(test_2.in ${CMAKE_RUNTIME_OUTPUT_DIRECTORY} COPYONLY)
configure_file(test_3.in ${CMAKE_RUNTIME_OUTPUT_DIRECTORY} COPYONLY)
