cmake_minimum_required(VERSION 3.10)

# Project name
project(UnixSocketIPC C)

# Use C standard
set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED ON)

# Add executables
add_executable(server_multiplexing AF_UNIX/multiplexing/server_multiplexing.c)
add_executable(server AF_UNIX/server.c)
add_executable(client AF_UNIX/client.c)
