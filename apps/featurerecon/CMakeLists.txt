file (GLOB HEADERS "*.h")
file (GLOB SOURCES "*.cc")

add_executable(featurerecon ${SOURCES} ${HEADERS})
target_link_libraries(featurerecon mve mve_util)
install(TARGETS featurerecon RUNTIME DESTINATION bin)