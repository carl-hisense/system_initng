INCLUDE_DIRECTORIES( ${CMAKE_SOURCE_DIR}/src ${CMAKE_BINARY_DIR} )

IF(SERVICE_CACHE)
	ADD_EXECUTABLE(test_parser test_parser.c)
	TARGET_LINK_LIBRARIES(test_parser initng)
ENDIF(SERVICE_CACHE)
