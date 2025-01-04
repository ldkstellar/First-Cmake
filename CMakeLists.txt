# 최소 CMake 버전 요구사항 명시
cmake_minimum_required(VERSION 3.0.0)

# 프로젝트 이름지정
project(hello-cmake)

# 컴파일러 설정
set(CMAKE_CXX_COMPILER clang++)

#[=[
{} cpp version 설정
set(CMAKE_CXX_STANDARD 03)
]=]#

# 타겟 프로그램정의
add_executable(hello_cmake src/main.cpp)

#조건문
if(BUILD_TESTING)
    message("Hello Test")
endif()
