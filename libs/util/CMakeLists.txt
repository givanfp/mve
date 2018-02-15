file (GLOB HEADERS "*.h")
file (GLOB SOURCES "[^_]*.cc")

add_library(mve_util STATIC ${SOURCES} ${HEADERS})
install(TARGETS mve_util DESTINATION lib)
install(FILES ${HEADERS} DESTINATION include/util)