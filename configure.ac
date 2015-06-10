dnl Process this file with autoconf to produce a configure script.

# get rid of that stupid cache mechanism
rm -f config.cache

m4_define([EPEG_MAJOR], 0)
m4_define([EPEG_MINOR], 9)
m4_define([EPEG_PATCH], 2)
m4_define([EPEG_CURRENT], 10)
m4_define([EPEG_REVISION], 0)
m4_define([EPEG_AGE], 10)

AC_INIT(epeg, [EPEG_MAJOR.EPEG_MINOR.EPEG_PATCH],
              [enlightenment-devel@lists.sourceforge.net], [epeg],
              [https://github.com/mattes/epeg])
AC_PREREQ(2.61)
AC_CONFIG_SRCDIR(configure.ac)

AM_INIT_AUTOMAKE([1.6 dist-bzip2])
AC_CONFIG_HEADERS([config.h])

LT_INIT([win32-dll])

AC_ISC_POSIX
AC_PROG_CC
AM_PROG_CC_STDC
AC_HEADER_STDC
AC_C_CONST

define([AC_LIBTOOL_LANG_CXX_CONFIG], [:])
define([AC_LIBTOOL_LANG_F77_CONFIG], [:])

# Define substitutions for the libtool version numbers.
EPEG_LT_CURRENT=EPEG_CURRENT
EPEG_LT_REVISION=EPEG_REVISION
EPEG_LT_AGE=EPEG_AGE
AC_SUBST(EPEG_LT_CURRENT)
AC_SUBST(EPEG_LT_REVISION)
AC_SUBST(EPEG_LT_AGE)

# AC_CHECK_FUNCS(fmemopen)
# AC_CHECK_FUNCS(open_memstream)

AC_CHECK_LIB([jpeg], [main], [], AC_MSG_ERROR([libjpeg library not found. Please install it before proceeding]))
AC_CHECK_LIB([exif], [main], [], AC_MSG_ERROR([libexif library not found. Please install it before proceeding]))

AC_OUTPUT([
    Makefile
    epeg.pc
    epeg-uninstalled.pc
    epeg.spec
    src/Makefile
    src/lib/Makefile
    src/bin/Makefile
])

