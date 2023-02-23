cmake_minimum_required (VERSION 3.8)

project (CPPM7_10)
add_library(CPPM7_10 CPPM7_10.cpp)
add_library(CPPM7_10_1 CPPM7_10_1.cpp)
add_library(CPPM7_10_2 CPPM7_10_2.cpp)
add_library(Figure Figure.cpp)
add_library(Triangle Triangle.cpp)
add_library(Quadrilateral Quadrilateral.cpp)

add_executable (CPPM7_10_exe CPPM7_10.cpp)

target_link_libraries(CPPM7_10_exe CPPM7_10)
target_link_libraries(CPPM7_10_exe CPPM7_10_1)
target_link_libraries(CPPM7_10_exe CPPM7_10_2)
target_link_libraries(CPPM7_10_2 Figure)
target_link_libraries(CPPM7_10_2 Triangle)
target_link_libraries(CPPM7_10_2 Quadrilateral)
