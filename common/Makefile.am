AM_CPPFLAGS = -I$(top_srcdir)/include

AM_CFLAGS = $(GLOBAL_CFLAGS) $(libplist_CFLAGS) $(LFS_CFLAGS)
AM_LDFLAGS = $(libplist_LIBS) ${libpthread_LIBS}

noinst_LTLIBRARIES = libinternalcommon.la
libinternalcommon_la_LIBADD = 
libinternalcommon_la_LDFLAGS = $(AM_LDFLAGS) -no-undefined
libinternalcommon_la_SOURCES = \
		       socket.c socket.h \
		       thread.c thread.h

if WIN32
libinternalcommon_la_LIBADD += -lole32
endif
