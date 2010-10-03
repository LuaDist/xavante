# Copyright (C) 2007-2010 LuaDist.
# Created by Peter Drahoš
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT(xavante NONE)
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
INCLUDE(dist.cmake)

INSTALL (FILES src/xavante/xavante.lua src/sajax/sajax.lua DESTINATION ${INSTALL_LMOD})
INSTALL (FILES
	src/xavante/cgiluahandler.lua
	src/xavante/encoding.lua
	src/xavante/filehandler.lua
	src/xavante/httpd.lua
	src/xavante/mime.lua
	src/xavante/patternhandler.lua
	src/xavante/redirecthandler.lua
	src/xavante/vhostshandler.lua
	src/xavante/indexhandler.lua
	src/xavante/urlhandler.lua
	src/xavante/ruleshandler.lua
	DESTINATION ${INSTALL_LMOD}/xavante )
INSTALL (FILES README DESTINATION ${INSTALL_DATA})
INSTALL (DIRECTORY doc/ DESTINATION ${INSTALL_DOC})
INSTALL (DIRECTORY examples/ DESTINATION ${INSTALL_EXAMPLE})
