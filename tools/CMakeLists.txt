cmake_minimum_required( VERSION 3.18.4 )

add_subdirectory( lemon )
add_subdirectory( re2c )
if( WIN32 AND NOT CMAKE_SIZEOF_VOID_P MATCHES "8" )
	add_subdirectory( fixrtext )
endif()
add_subdirectory( zipdir )

set( CROSS_EXPORTS ${CROSS_EXPORTS} PARENT_SCOPE )
