## Process this file with automake to produce Makefile.in

SUBDIRS = src

MAINTAINERCLEANFILES = Makefile.in aclocal.m4 config.guess \
                       config.h.in config.sub configure install-sh \
		       ltconfig ltmain.sh missing mkinstalldirs \
		       stamp-h.in epeg.c depcomp \
		       epeg.spec

EXTRA_DIST = README AUTHORS COPYING COPYING-PLAIN \
	     autogen.sh epeg.spec epeg.spec.in epeg.c.in gendoc \
	     Doxyfile README.md

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = epeg.pc
