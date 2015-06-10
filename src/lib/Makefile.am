
MAINTAINERCLEANFILES = Makefile.in

lib_LTLIBRARIES      = libepeg.la
include_HEADERS      = Epeg.h
libepeg_la_SOURCES = \
	epeg_main.c \
	epeg_private.h

libepeg_la_DEPENDENCIES = $(top_builddir)/config.h
libepeg_la_LDFLAGS      = -version-info $(EPEG_LT_CURRENT):$(EPEG_LT_REVISION):$(EPEG_LT_AGE)

