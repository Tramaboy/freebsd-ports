# Created by: Remington Lang <MrL0Lz@gmail.com>
# $FreeBSD$

PORTNAME=	gcfilms
PORTVERSION=	6.4
PORTREVISION=	4
CATEGORIES=	multimedia perl5
MASTER_SITES=	http://download.gna.org/gcfilms/

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Tool to manage movie collections

LICENSE=	GPLv2
LICENSE_FILE=	${WRKSRC}/LICENSE

BROKEN=		unfetchable
DEPRECATED=	Unfetchable, unmaintained
EXPIRATION_DATE=	2019-10-16

BUILD_DEPENDS=	p5-XML-Simple>=0:textproc/p5-XML-Simple \
		p5-Gtk2>=0:x11-toolkits/p5-Gtk2 \
		p5-HTML-Parser>=0:www/p5-HTML-Parser \
		p5-libwww>=0:www/p5-libwww
RUN_DEPENDS:=	${BUILD_DEPENDS}

WRKSRC=		${WRKDIR}/${PORTNAME}

NO_ARCH=	yes
NO_BUILD=	yes
USES=		shebangfix

SHEBANG_FILES=	bin/gcfilms install

do-install:
	cd ${WRKSRC} ; ./install --prefix=${STAGEDIR}${PREFIX}

.include <bsd.port.mk>
