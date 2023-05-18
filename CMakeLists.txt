cmake_minimum_required(VERSION 3.14)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
project("projekt")
# file(GLOB_RECURSE SOURCES *.cpp)



add_executable(${PROJECT_NAME} main.cpp 
    Klasa.cpp
    klasy/Klasa2.cpp
)