# Created by: Alex Dupre <ale@FreeBSD.org>
# $FreeBSD$

PORTNAME=	pdflib
PORTVERSION=	4.1.3
CATEGORIES=	print pear

MAINTAINER=	ale@FreeBSD.org
COMMENT=	PECL extension to create PDF on the fly

LICENSE=	PHP30

LIB_DEPENDS=	libpdf.so:print/pdflib

USES=		php:pecl
USE_PHP=	gd:build
PHP_MODNAME=	pdf

CONFIGURE_ARGS=	--with-pdflib=${LOCALBASE}

.include <bsd.port.mk>
