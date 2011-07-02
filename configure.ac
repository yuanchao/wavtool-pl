# Process this file with autoconf to produce a configure script.
AC_INIT(wavtool-pl, 0.1, paulliu@debian.org)
AM_CONFIG_HEADER(config.h)
AM_INIT_AUTOMAKE(wavtool-pl,0.1)

# Checks for programs.
AC_PROG_AWK
AC_PROG_CC
AC_PROG_INSTALL
AC_PROG_LN_S
AM_PROG_CC_C_O

# Checks for libraries.
AC_HAVE_LIBRARY([m])

# Checks for header files.
AC_HEADER_SYS_WAIT
AC_HEADER_STDC
AC_UNISTD_H

# Checks for typedefs, structures, and compiler characteristics.
AC_C_CONST

# Checks for library functions.
AC_FUNC_FORK
AC_FUNC_MEMCMP
AC_TYPE_SIGNAL
AC_CHECK_FUNCS([memset])

# Check Packages
PKG_CHECK_MODULES(SNDFILE, [sndfile])
AC_SUBST(SNDFILE_CFLAGS)
AC_SUBST(SNDFILE_LIBS)

AC_CONFIG_FILES([
Makefile
src/Makefile
])
AC_OUTPUT
