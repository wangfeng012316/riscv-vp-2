file(GLOB_RECURSE HEADERS ${CMAKE_CURRENT_SOURCE_DIR}/*.h)

add_library(platform-common
		fe310_plic.cpp
		fu540_plic.cpp
        ${HEADERS})

target_include_directories(platform-common PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
