ADD_LIBRARY(student student.h student.cpp)

ADD_EXECUTABLE(demo demo.cpp)

TARGET_LINK_LIBRARIES(demo student)
