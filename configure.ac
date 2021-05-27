AC_PREREQ(2.52)

AC_INIT([Apertium Italian-Portuguese], [0.0.1], [apertium-stuff@lists.sourceforge.net], [apertium-ita-por], [https://wiki.apertium.org/wiki/Apertium-ita-por])
AM_INIT_AUTOMAKE
AC_PROG_AWK

PKG_CHECK_MODULES(APERTIUM, apertium >= 3.6.1)
PKG_CHECK_MODULES(LTTOOLBOX, lttoolbox >= 3.5.1)

AC_PATH_PROGS(ZCAT, [gzcat zcat], [false])
AS_IF([test x$ZCAT = xfalse], [AC_MSG_ERROR([You don't have zcat nor gzcat installed])])

m4_ifdef([AP_CHECK_LING],[],[AC_MSG_ERROR([AP_CHECK_LING not defined, is apertium.m4 in ACLOCAL_PATH? See: https://wiki.apertium.org/wiki/Installation_troubleshooting])])


#AP_CHECK_LING([1], [apertium-ita])

#AP_CHECK_LING([2], [apertium-por])

AP_MKINCLUDE

AC_OUTPUT([Makefile])
