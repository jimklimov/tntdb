AM_CPPFLAGS = @PG_CPPFLAGS@ -I$(top_srcdir)/include -I$(top_builddir)/include

sources = connection.cpp connectionmanager.cpp cursor.cpp error.cpp result.cpp resultrow.cpp resultvalue.cpp statement.cpp

if MAKE_POSTGRESQL

driver_LTLIBRARIES = tntdb@abi_current@-postgresql.la

tntdb@abi_current@_postgresql_la_SOURCES = $(sources)
tntdb@abi_current@_postgresql_la_LDFLAGS = -module -version-info @sonumber@ @PG_LDFLAGS@ @SHARED_LIB_FLAG@
tntdb@abi_current@_postgresql_la_LIBADD = $(top_builddir)/src/libtntdb.la

endif
