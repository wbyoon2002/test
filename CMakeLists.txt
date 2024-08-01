cmake_minimum_required(VERSION 3.5.0) # 최소요구버전
project(test_cmake VERSION 0.1.0) # PROJECT_NAME 과 PROJECT_VERSION

add_executable(test_cmake cpp/src/main.cpp cpp/src/Test.cpp) # 빌드 대상 추가. [실행파일명] [소스파일명] [소스파일명]

set(CPACK_PROJECT_NAME ${PROJECT_NAME}) # 실행파일명
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION}) # 실행파일버전
include(CPack) # 기본적으로 build 경로에 실행파일을 생성함