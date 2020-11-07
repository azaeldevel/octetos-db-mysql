AUTOMAKE_OPTIONS=foreign 1.4


if WITH_DEBIAN
DEFINESO = -DLINUX_DEBIAN
endif


lib_LTLIBRARIES = liboctetos-db-mysql.la

liboctetos_db_mysql_la_LIBADD = $(MYSQLCLIENT_LIBS)
liboctetos_db_mysql_la_CXXFLAGS = $(MYSQLCLIENT_CFLAGS) $(DEFINESO)
liboctetos_db_mysql_la_SOURCES = clientdb-mysql.cc

octetos_db_includedir = $(includedir)/octetos/db
pkgconfigdir = $(libdir)/pkgconfig
octetos_db_include_HEADERS = clientdb-mysql.hh
pkgconfig_DATA = octetos-db-mysql.pc
EXTRA_DIST = octetos-db-mysql.pc.in