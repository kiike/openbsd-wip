# $OpenBSD: Makefile.template,v 1.72 2015/04/08 17:53:19 sthen Exp $

COMMENT =		shell frontend for duplicity backup tool

V =			1.11.1
DISTNAME =		duply_${V}
PKGNAME =		duply-${V}

CATEGORIES =		sysutils

HOMEPAGE =		http://duply.net/

# GPLv2
PERMIT_PACKAGE_CDROM =	Yes

# XXX should use ${MASTER_SITE_SOURCEFORGE:=ftplicity/} but % in the
# XXX path causes problems
MASTER_SITES =		http://downloads.sourceforge.net/project/ftplicity/duply%20%28simple%20duplicity%29/1.11.x/
#MASTER_SITES =		${MASTER_SITE_SOURCEFORGE:=ftplicity/'duply%20%28simple%20duplicity%29'/1.9.x/}

EXTRACT_SUFX =		.tgz

RUN_DEPENDS =		shells/bash \
			sysutils/duplicity \
			security/gnupg<2

NO_BUILD =		Yes
NO_TEST =		Yes

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/duply ${PREFIX}/bin/duply

.include <bsd.port.mk>
