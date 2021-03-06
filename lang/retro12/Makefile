# $FreeBSD$

PORTNAME=	retro12
DISTVERSION=	2019.7
CATEGORIES=	lang
MASTER_SITES=	http://forthworks.com/retro/r/ \
		https://forthworks.com/retro/r/
DISTNAME=	${PORTNAME:tu}-${DISTVERSION}

MAINTAINER=	0mp@FreeBSD.org
COMMENT=	Clean, elegant, and pragmatic dialect of Forth

LICENSE=	ISCL
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=	ncurses shebangfix

SHEBANG_FILES=	example/Atua*
SHEBANG_LANG=	retro

MAKE_ENV=	DATADIR=${DATADIR} \
		DESTDIR=${DESTDIR} \
		DOCSDIR=${DOCSDIR} \
		EXAMPLESDIR=${EXAMPLESDIR} \
		PREFIX=${PREFIX}
# There are race conditions in the makefile due to missing dependencies for
# targets as upstream tests releases on single core machines.
MAKE_JOBS_UNSAFE=	yes

PLIST_FILES=	bin/retro \
		bin/retro-describe \
		bin/retro-document \
		bin/retro-embedimage \
		bin/retro-extend \
		bin/retro-muri \
		bin/retro-unu

PORTDATA=	glossary.forth \
		ngaImage \
		tests \
		words.tsv

PORTDOCS=	doc \
		README \
		RELEASE-NOTES

PORTEXAMPLES=	example

INSTALL_TARGET=	install-strip
TEST_TARGET=	test

OPTIONS_DEFINE=	DOCS EXAMPLES

.include <bsd.port.mk>
