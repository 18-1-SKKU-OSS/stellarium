
########### install files ###############

# install landscape.ini
INSTALL (FILES landscape.ini DESTINATION share/${PACKAGE}/landscapes/geneva )

# install textures and descriptions
INSTALL (DIRECTORY ./ DESTINATION share/${PACKAGE}/landscapes/geneva 
	FILES_MATCHING PATTERN "*.txt" 
	PATTERN "description.*.utf8" 
	PATTERN "CMake*" EXCLUDE )
