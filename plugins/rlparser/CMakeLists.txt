INCLUDE_DIRECTORIES( ${CMAKE_SOURCE_DIR}/src ${CMAKE_BINARY_DIR} )

ADD_LIBRARY(rlparser MODULE initng_rl_parser.c)
TARGET_LINK_LIBRARIES(rlparser initng)
INSTALL_TARGETS(${LIB_INSTALL_DIR}/initng rlparser)

