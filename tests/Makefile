#
LOCALBASE?=	/usr/local
PROGS=		pool_test
.ifdef USE_STR
PROGS+=		str_test
.endif

CFLAGS=		-I${.CURDIR}/../src \
		-I${.CURDIR}/

LDFLAGS+=	-L${.CURDIR}/../src

LDADD=		-lpool

MAN=
MK_DEBUG_FILES=	no
MAKEOBJDIR= .

# keep this empty otherwise installation fails
install:

test:
	./pool_test
.ifdef USE_STR
	./str_test
.endif

.include <bsd.progs.mk>
