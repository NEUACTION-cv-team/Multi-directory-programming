﻿# cmake version
cmake_minimum_required(VERSION 3.0)

aux_source_directory(. DIR_SRCS)
add_executable(lidar ${DIR_SRCS})

include_directories(${PROCESS_COMM_DIR})
target_link_libraries(lidar process_communication)
