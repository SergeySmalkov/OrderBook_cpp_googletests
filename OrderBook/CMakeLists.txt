project(OrderBook)


set(HEADER_FILES OrderBook.h)
set(SOURCE_FILES OrderBook.cpp)

add_library(OrderBook_lib STATIC ${SOURCE_FILES} ${HEADER_FILES})