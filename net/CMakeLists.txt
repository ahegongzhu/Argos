cmake_minimum_required(VERSION 2.8)
set(SOURCE_LIST)
file(GLOB H_LIST "*.h")
file(GLOB HPP_LIST "*.hpp")
file(GLOB CPP_LIST "*.cpp")
list(APPEND SOURCE_LIST ${H_LIST} ${HPP_LIST} ${CPP_LIST})
add_library(net STATIC ${SOURCE_LIST})
