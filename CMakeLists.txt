# set the minimum version for cmake
CMAKE_MINIMUM_REQUIRED(VERSION  2.8)

# set the project name
PROJECT(cmake_test)

# directive to print detail build log
SET(CMAKE_VERBOSE_MAKEFILE ON)

# set the output directory for bin during building(make)
SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)

# set the output directory for libs during building(make)
SET(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)

# 可以分离dll和lib
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)

# 包含头文件搜索路径
INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/include) 

# 包含库搜索路径
LINK_DIRECTORIES(${PROJECT_SOURCE_DIR}/lib)

# 子文件夹
ADD_SUBDIRECTORY(src)

# 子文件夹
ADD_SUBDIRECTORY(test)