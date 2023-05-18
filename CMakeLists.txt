cmake_minimum_required(VERSION 3.14)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
project("projekt")
# file(GLOB_RECURSE SOURCES *.cpp) - be




add_library(${PROJECT_NAME}_lib
    "Klasa.cpp"
    "klasy/Klasa2.cpp"
)

target_include_directories(${PROJECT_NAME}_lib PRIVATE "klasy")

add_executable(${PROJECT_NAME} "main.cpp")
target_link_libraries(${PROJECT_NAME} PRIVATE ${PROJECT_NAME}_lib)

# tests
add_subdirectory("lib/cpputest")
add_subdirectory("tests")

