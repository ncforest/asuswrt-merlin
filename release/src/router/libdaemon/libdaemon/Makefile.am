# This file is part of libdaemon.
#
# Copyright 2003-2008 Lennart Poettering
#
# libdaemon is free software; you can redistribute it and/or modify it
# under the terms of the GNU Lesser General Public License as
# published by the Free Software Foundation, either version 2.1 of the
# License, or (at your option) any later version.
#
# libdaemon is distributed in the hope that it will be useful, but
# WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
# Lesser General Public License for more details.
#
# You should have received a copy of the GNU Lesser General Public
# License along with libdaemon. If not, see
# <http://www.gnu.org/licenses/>.

AM_CPPFLAGS='-DLOCALSTATEDIR="$(localstatedir)"'

pkginclude_HEADERS = \
	dlog.h \
	dfork.h \
	dsignal.h \
	dnonblock.h \
	dpid.h \
	dexec.h \
	daemon.h

lib_LTLIBRARIES = libdaemon.la

libdaemon_la_SOURCES = \
	dlog.c \
	dfork.c \
	dsignal.c \
	dnonblock.c \
	dpid.c \
	dexec.c \
	daemon.h \
	$(pkg_include_HEADERS)

libdaemon_la_LDFLAGS = -version-info $(LIBDAEMON_VERSION_INFO) $(LDFLAGS_NOUNDEFINED)
