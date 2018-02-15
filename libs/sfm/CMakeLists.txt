file (GLOB HEADERS "*.h")
file (GLOB SOURCES "[^_]*.cc")

add_library(mve_sfm STATIC ${SOURCES} ${HEADERS})
target_link_libraries(mve_sfm mve)
install(TARGETS mve_sfm DESTINATION lib)
install(FILES ${HEADERS} DESTINATION include/sfm)