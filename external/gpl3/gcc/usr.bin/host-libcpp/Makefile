#	$NetBSD: Makefile,v 1.2.6.1 2017/07/05 15:56:58 martin Exp $

libcpp/libcpp.a:
	[ ! -d libcpp ] && mkdir libcpp || true
	(cd libcpp; \
		CC=${HOST_CC:Q} CXX=${HOST_CXX:Q}  \
		CFLAGS=${HOST_CFLAGS:Q} \
		MAKE=${TOOL_GMAKE:Q} \
		CONFIG_SHELL=${HOST_SH:Q} \
		${HOST_SH} ${DIST}/libcpp/configure -v am_cv_func_iconv=no \
		&& CC=${HOST_CC:Q} CXX=${HOST_CXX:Q} CFLAGS=${HOST_CFLAGS:Q} ${TOOL_GMAKE})

cleandir:
	-rm -rf libcpp

depend dependall all: libcpp/libcpp.a

.include <bsd.prog.mk>
