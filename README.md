#slam_code_study
#19.10.31
1.在主目录下的CMakeLists.txt中需要添加项目名，cmake版本等等，即
  cmake_minimum_required(VERSION 2.8)
  project(slam_code_study)
  set(CMAKE_CXX_FLAGS "-fPIC")
  set(CMAKE_BUILD_TYPE "Debug")
  set(CMAKE_CXX_STANDARD 11)
  要添加需要编译的另外两个子文件夹src_bin,bin，则需要语句
  add_subdirectory(src)
  add_subdirectory(src_bin)

2.src里的CMakeLists.txt不需要添加项目名，cmake版本等等这些了

3.src_bin里的cmakelists.txt文件
  #target_link_libraries(helloSLAM helloSLAM_shared)#这样是相当于直接从build里面找到编译中间过程的文件
  target_link_libraries(helloSLAM ${PROJECT_SOURCE_DIR}/lib/libhelloSLAM_shared.so)#这样也可以，相当于调用第三方的共享库来编译