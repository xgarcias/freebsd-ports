# Created by: Jose Alonso Cardenas Marquez <acm@FreeBSD.org>
# $FreeBSD$

PORTNAME=	mupen64plus
PORTVERSION?=	2.5
PORTREVISION?=	1
CATEGORIES=	emulators
MASTER_SITES=	https://github.com/${PORTNAME}/${PORTNAME}${PKGNAMESUFFIX}/releases/download/${PORTVERSION}/ \
		LOCAL/acm/${PORTNAME} \
		LOCAL/acm/${PORTNAME}/:plugin
PKGNAMESUFFIX?=	-core
DIST_SUBDIR=	${PORTNAME}

MAINTAINER?=	acm@FreeBSD.org
COMMENT?=	Fork of Mupen64 Nintendo 64 emulator

USES+=		gmake pkgconfig
USE_GL?=	yes
USE_SDL?=	sdl2
USE_LDCONFIG?=	yes
ONLY_FOR_ARCHS=	i386 amd64

OPTFLAGS=	#

MAKE_ENV+=	OPTFLAGS="${OPTFLAGS}"

.include "${.CURDIR}/../mupen64plus-core/Makefile.common"
.include <bsd.port.mk>
