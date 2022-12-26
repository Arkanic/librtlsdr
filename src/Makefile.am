# This is _NOT_ the library release version, it's an API version.
# Please read Chapter 6 "Library interface versions" of the libtool documentation before making any modification
LIBVERSION=0:5:0

AUTOMAKE_OPTIONS = subdir-objects
INCLUDES = $(all_includes) -I$(top_srcdir)/include
noinst_HEADERS = convenience/convenience.h
AM_CFLAGS = ${CFLAGS} -fPIC ${SYMBOL_VISIBILITY}

lib_LTLIBRARIES = librtlsdr.la

librtlsdr_la_SOURCES = librtlsdr.c tuner_e4k.c tuner_fc0012.c tuner_fc0013.c tuner_fc2580.c tuner_r82xx.c
librtlsdr_la_LDFLAGS = -version-info $(LIBVERSION)
