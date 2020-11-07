

AC_INIT(octetos-db-mysql, 0.1.0-alpha,azael.devel@gmail.com)

AC_CONFIG_HEADERS([config.h])

AM_INIT_AUTOMAKE([1.11])

AM_SILENT_RULES([yes])

AC_PROG_CXX



AC_ARG_WITH([debian], AS_HELP_STRING([--with-debian], [Activating compilation for Debian.]))
AM_CONDITIONAL(WITH_DEBIAN, test x"$with_debian" = "xyes")





LT_INIT

PKG_CHECK_MODULES(MYSQLCLIENT, mysqlclient)




AC_OUTPUT([
Makefile
src/Makefile
src/octetos-db-mysql.pc
])
