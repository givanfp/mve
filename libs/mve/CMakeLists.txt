file (GLOB HEADERS "*.h")
file (GLOB SOURCES "[^_]*.cc")

add_library(mve STATIC ${SOURCES} ${HEADERS})
target_link_libraries(mve ${JPEG_LIBRARIES} ${PNG_LIBRARIES} ${TIFF_LIBRARIES})
install(TARGETS mve DESTINATION lib)
install(FILES ${HEADERS} DESTINATION include/mve)