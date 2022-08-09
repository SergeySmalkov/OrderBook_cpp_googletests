cmake_minimum_required(VERSION 3.21)
project(OrderBookDemo)

set(CMAKE_CXX_STANDARD 20)

set(SOURCE_FILES main.cpp)
add_executable(OrderBookDemo ${SOURCE_FILES})

include_directories(OrderBook)
add_subdirectory(OrderBook)

add_subdirectory(OrderBookTests)

target_link_libraries(OrderBookDemo OrderBook_lib)

