cmake_minimum_required (VERSION 2.8)
project(loitorusbcam)
set(CMAKE_C_COMPILER g++)

link_directories("../loitorimu")

add_library(loitorusbcam STATIC loitorusbcam.cpp)
target_link_libraries(loitorusbcam loitorimu)
