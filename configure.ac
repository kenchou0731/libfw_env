# libfw_env version
m4_define([version_major], [1])
m4_define([version_minor], [0])
m4_define([version_revision], [0])
m4_define([version_code], [version_major.version_minor.version_revision])

# autoconf, automake, libtool initial
AC_PREREQ(2.69)
AC_INIT([libfw_env], [version_code])
AM_INIT_AUTOMAKE

AM_SILENT_RULES([yes])

LT_PREREQ(2.4)
LT_INIT

VERSION_CODE=version_code
AC_SUBST(VERSION_CODE)

# check libraries & headers
AC_DEFUN([FUNC_NOT_FOUND_LIB],
	[AC_MSG_ERROR([library $1 not found])])
AC_DEFUN([HEADER_NOT_FOUND_LIB],
	[AC_MSG_ERROR([header $1 not found])])

# output
AC_CONFIG_FILES([
	include/Makefile
	lib/Makefile
	Makefile
])
AC_OUTPUT
