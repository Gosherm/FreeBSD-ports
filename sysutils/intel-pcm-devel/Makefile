# Created by: Adrian Chadd
# $FreeBSD$

PORTNAME=	intel-pcm
DISTVERSION=	g20200902
PORTEPOCH=	1
CATEGORIES=	sysutils
PKGNAMESUFFIX=	-devel

MAINTAINER=	egypcio@FreeBSD.org
COMMENT=	Process Count Monitor (PCM) for Intel processors

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

ONLY_FOR_ARCHS=	amd64 i386

USES=		gmake
USE_GITHUB=	yes

GH_ACCOUNT=	opcm
GH_PROJECT=	pcm
GH_TAGNAME=	40d3b77

PORTSCOUT=	skipv:202008,202009

CONFLICTS_INSTALL=	intel-pcm

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/*.x ${STAGEDIR}${PREFIX}/sbin

.include <bsd.port.mk>
