ADD_LIBRARY(student student.h student.cpp)

ADD_EXECUTABLE(demo demo.cpp)

TARGET_LINK_LIBRARIES(demo student)

ADD_EXECUTABLE(test2 test2.cpp)
TARGET_LINK_LIBRARIES(test2 student)
