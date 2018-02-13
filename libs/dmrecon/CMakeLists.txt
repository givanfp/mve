file (GLOB HEADERS "*.h")
file (GLOB SOURCES "[^_]*.cc")

add_library(mve_dmrecon STATIC ${SOURCES} ${HEADERS})
install(TARGETS mve_dmrecon DESTINATION lib)