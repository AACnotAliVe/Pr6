cmake_minimum_required(VERSION 3.5.2)
project(JasonVoorhes)

set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED ON)

find_package(Threads REQUIRED)

add_executable(z1 z1.c)
add_executable(z2 z2.c)

target_link_libraries(z1 Threads::Threads)
target_link_libraries(z2 Threads::Threads)
