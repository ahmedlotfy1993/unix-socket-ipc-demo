cmake_minimum_required(VERSION 3.10)

# Project name
project(UnixSocketIPC C)

# Use C standard
set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED ON)

# Add executables
add_executable(server server.c)
add_executable(client client.c)
