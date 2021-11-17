cmake_minimum_required(VERSION 3.10)

project(Sift_Opencv)
set(CMAKE_BUILD_TYPE "Debug")
set(OpenCV_DIR "E:\\Code_repositories\\opencv\\build\\x64\\vc14\\lib") # 错误修正
find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable(Sift_Opencv "main.cpp") # 错误修正
target_link_libraries(Sift_Opencv ${OpenCV_LIBS})