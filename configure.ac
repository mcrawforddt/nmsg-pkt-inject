#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.71])
AC_INIT([nmsg-pkt-inject],[0.3.0],[software@farsightsecurity.com])
AM_INIT_AUTOMAKE([-Wall -Werror foreign])
AC_CONFIG_SRCDIR([argv.h])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CC


# Checks for libraries.
# FIXME: Replace 'main' with a function in '-lnmsg':
AC_CHECK_LIB([nmsg], [main])
# FIXME: Replace 'main' with a function in '-lpcap':
AC_CHECK_LIB([pcap], [main])
# FIXME: Replace 'main' with a function in '-lpthread':
AC_CHECK_LIB([pthread], [main])

# Checks for header files.
AC_CHECK_HEADERS([arpa/inet.h stdint.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_HEADER_STDBOOL
AC_C_INLINE

# Checks for library functions.
AC_FUNC_MALLOC
AC_FUNC_REALLOC
AC_CHECK_FUNCS([strchr])

AC_CONFIG_FILES([Makefile])
AC_OUTPUT
