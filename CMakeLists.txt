cmake_minimum_required(VERSION 3.10)

project(gerenciadorDeFinancias)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Curses REQUIRED)

add_executable(meu_programa main.cpp)

target_include_directories(meu_programa PRIVATE ${CURSES_INCLUDE_DIR})
target_link_libraries(meu_programa PRIVATE ${CURSES_LIBRARIES})
