# Maintainer makefile for Automake-NG.

# Copyright (C) 2012 Free Software Foundation, Inc.
#
# This program is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; either version 2, or (at your option)
# any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.

# If the user runs GNU make but has not yet run ./configure,
# give them an helpful diagnostic instead of a cryptic error.
am--Makefile := $(wildcard Makefile)
ifeq ($(am--Makefile),)
  $(warning There seems to be no Makefile in this directory.)
  $(warning You must run ./configure before running 'make'.)
  $(error Fatal Error)
else
  include ./Makefile
  include $(srcdir)/syntax-checks.mk
endif