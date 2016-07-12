cmake_minimum_required(VERSION 2.8)
project(SerialTest)
find_package(serial REQUIRED)

add_executable(${PROJECT_NAME} SerialTest.cpp)
include_directories(${serial_INCLUDE_DIRS})
target_link_libraries(${PROJECT_NAME} serial)
