#
MK_PROFILE=	no
LOCALBASE?=	/usr/local
LIB=            pool
LIBDIR=		${LOCALBASE}/lib
INCSDIR=	${LOCALBASE}/include
CFLAGS+=        -Wall -Wstrict-prototypes -fPIC -I${.CURDIR}
SRCS=		pool.c libpool.h
.ifdef USE_STR
CFLAGS+= -DUSE_STR
SRCS+=		misc.c \
		str.c
.endif

INCS=		libpool.h

NO_OBJ=         yes

.include <bsd.lib.mk>
