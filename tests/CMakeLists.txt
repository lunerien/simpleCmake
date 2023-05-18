cmake_minimum_required(VERSION 3.14)
project("projekt_test")

add_executable(${PROJECT_NAME} "mainTests.cpp"
    "Testy.cpp"
    "../klasy/Klasa2.cpp"
)

target_link_libraries(${PROJECT_NAME} PRIVATE CppUTest)