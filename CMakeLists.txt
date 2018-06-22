cmake_minimum_required(VERSION 2.8)

ENABLE_TESTING()

ADD_LIBRARY(student student.h student.cpp)

ADD_EXECUTABLE(demo demo.cpp)
TARGET_LINK_LIBRARIES(demo student)

ADD_EXECUTABLE(test1 test1.cpp)
TARGET_LINK_LIBRARIES(test1 student)
ADD_TEST(test1 test1)

