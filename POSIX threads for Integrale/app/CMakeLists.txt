CMAKE_MINIMUM_REQUIRED(VERSION 2.8)
PROJECT(Integral C)
SET(TARGET_NAME Integral)
AUX_SOURCE_DIRECTORY(. SRC)
ADD_EXECUTABLE(Integral ${SRC})
TARGET_LINK_LIBRARIES(${TARGET_NAME} m)
SET(CMAKE_C_FLAGS "-lpthread -fopenmp -lm -O3")