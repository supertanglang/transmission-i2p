AM_CPPFLAGS = -I@top_srcdir@

AM_CFLAGS = \
    @LIBEVENT_CFLAGS@ \
    @OPENSSL_CFLAGS@ \
    @LIBCURL_CFLAGS@ \
    @ZLIB_CFLAGS@ \
    @PTHREAD_CFLAGS@

AM_LDFLAGS = \
    @ZLIB_LDFLAGS@

bin_PROGRAMS = transmission-cli

dist_man_MANS = transmission-cli.1

transmission_cli_SOURCES = cli.c

transmission_cli_LDADD = \
    $(top_builddir)/libtransmission/libtransmission.a \
    $(top_builddir)/third-party/libbob/libbob.a \
    $(top_builddir)/third-party/libsam3/libsam3.a \
    @LIBNATPMP_LIBS@ \
    @LIBUPNP_LIBS@ \
    @DHT_LIBS@ \
    @LIBUTP_LIBS@ \
    @LIBEVENT_LIBS@ \
    @LIBCURL_LIBS@ \
    @OPENSSL_LIBS@ \
    @INTLLIBS@ \
    @ZLIB_LIBS@ \
    @PTHREAD_LIBS@

