set(HEADERS 
            ${PROJECT_SOURCE_DIR}/include/libHelloSLAM.h
            #libHelloSLAM.h
   )
set(SOURCES_FILES
            libHelloSLAM.cpp
   )
set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib )

add_library(helloSLAM_shared SHARED ${HEADERS} ${SOURCES_FILES})

