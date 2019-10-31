set(EXECUTABLE_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/bin)

add_executable(helloSLAM useHello.cpp)

target_link_libraries(helloSLAM ${PROJECT_SOURCE_DIR}/lib/libhelloSLAM_shared.so)#这样也可以，相当于调用第三方的共享库来编译

#target_link_libraries(helloSLAM helloSLAM_shared)#这样是相当于直接从build里面找到编译中间过程的文件