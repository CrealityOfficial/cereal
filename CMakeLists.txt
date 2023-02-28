cmake_minimum_required (VERSION 2.6.2)


if(CC_INSTALL_CEREAL)
	__install_directory_specif(${CMAKE_CURRENT_SOURCE_DIR}/include/ cereal)
endif()

add_library(cereal INTERFACE)
set_property(TARGET cereal PROPERTY INTERFACE_INCLUDE_DIRECTORIES ${CMAKE_CURRENT_SOURCE_DIR}/include/)
