cmake_minimum_required(VERSION 3.20)

project(3D_renderer VERSION 1.0)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

cmake_policy(SET CMP0148 NEW)

add_executable(3D_renderer 
    src/main.cpp 
)

set_target_properties(3D_renderer PROPERTIES 
    RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_SOURCE_DIR}/lib"
)

target_include_directories(3D_renderer PRIVATE "${CMAKE_CURRENT_SOURCE_DIR}/include")