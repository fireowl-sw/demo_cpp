cmake_minimum_required(VERSION 3.10)
project(firewol)  # 项目名称

set(CMAKE_CXX_STANDARD 17)  # 指定 C++ 标准

# 添加可执行文件（自动搜索 src 下的所有 .cpp）
file(GLOB SOURCES "src/*.cpp")
add_executable(${PROJECT_NAME} ${SOURCES})

# 包含头文件目录（如果有）
include_directories(include)