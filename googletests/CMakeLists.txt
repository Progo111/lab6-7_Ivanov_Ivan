cmake_minimum_required(VERSION 3.16)

add_executable(testing test.cpp)

target_link_libraries(testing
        gtest
        gtest_main
        pthread
        header.hpp)

add_test(
        NAME testing
        COMMAND testing
)