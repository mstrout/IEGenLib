## Process this file with automake to generate Makefile.in

# Copyright 2001, 2002, 2003, 2009, 2010, 2012 Free Software Foundation, Inc.
#
# This file is part of the GNU MP Library.
#
# The GNU MP Library is free software; you can redistribute it and/or modify
# it under the terms of the GNU Lesser General Public License as published by
# the Free Software Foundation; either version 3 of the License, or (at your
# option) any later version.
#
# The GNU MP Library is distributed in the hope that it will be useful, but
# WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
# or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public
# License for more details.
#
# You should have received a copy of the GNU Lesser General Public License
# along with the GNU MP Library.  If not, see http://www.gnu.org/licenses/.


INCLUDES = -I$(top_srcdir) -I$(top_srcdir)/tests
LDADD = $(top_builddir)/tests/libtests.la $(top_builddir)/libgmp.la

check_PROGRAMS = t-asmtype t-aors_1 t-divrem_1 t-mod_1 t-fat t-get_d	\
  t-instrument t-iord_u t-mp_bases t-perfsqr t-scan logic		\
  t-toom22 t-toom32 t-toom33 t-toom42 t-toom43 t-toom44			\
  t-toom52 t-toom53 t-toom62 t-toom63 t-toom6h t-toom8h			\
  t-mul t-mullo t-mulmod_bnm1 t-sqrmod_bnm1				\
  t-hgcd t-matrix22 t-invert t-div t-bdiv

EXTRA_DIST = toom-shared.h

TESTS = $(check_PROGRAMS)

$(top_builddir)/tests/libtests.la:
	cd $(top_builddir)/tests; $(MAKE) $(AM_MAKEFLAGS) libtests.la
