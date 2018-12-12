#共享库
ADD_LIBRARY(ttt SHARED test.cpp)
#链接库
target_link_libraries(ttt optimized opencv_world330)
target_link_libraries(ttt debug opencv_world330d)