dnl Process this file with autoconf to produce a configure script.

AC_PREREQ(2.50)
AC_INIT(runtest.exp)
AM_INIT_AUTOMAKE(dejagnu, 1.4.4)
AM_MAINTAINER_MODE
AC_PROG_MAKE_SET

AC_PROG_CC
AC_PROG_CXX
AC_PROG_INSTALL
AC_EXEEXT

AC_PROG_YACC

dnl we need the path to Docbook so we can build packages.
DJ_AC_PATH_DOCBOOK

dnl we need the path to the tcl shell to build a release
DJ_AC_PATH_TCLSH

dnl Level of indirection for automake macro (baseboards:boards_DATA)
BOARDS='$(boards)'
AC_SUBST(BOARDS)
CONFIG='$(config)'
AC_SUBST(CONFIG)

AC_CONFIG_SUBDIRS(example/calc example/hello)

AC_OUTPUT(Makefile doc/Makefile testsuite/Makefile example/Makefile
          testsuite/libdejagnu/Makefile)