cmake_minimum_required(VERSION 3.25)
project(TestPDCurses)

set(CMAKE_CXX_STANDARD 20)

find_package(unofficial-pdcurses CONFIG REQUIRED)
add_executable(TestPDCurses main.cpp)

target_link_libraries(TestPDCurses PRIVATE unofficial::pdcurses::pdcurses)
