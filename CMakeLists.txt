cmake_minimum_required(VERSION 3.5)
project(BCD_Planner)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++14")

find_package(OpenCV REQUIRED)
include_directories(OpenCV_INCLUDE_DIRS)
include_directories(/usr/include/eigen3)

#add_executable(BCD_Planner main.cpp a-star.h)
add_executable(BCD_Planner main.cpp)
target_link_libraries(BCD_Planner ${OpenCV_LIBS})