cmake_minimum_required(VERSION 3.22.1)
project(cpp-graph-project VERSION 0)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_subdirectory(mgclient)

include_directories(/usr/lib/llvm-14/include)

add_library(mgclient INTERFACE)
target_include_directories(mgclient INTERFACE mgclient/mgclient_cpp/include)
target_link_libraries(mgclient INTERFACE mgclient-static)

add_subdirectory(cpp-graph)
