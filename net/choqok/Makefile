# $NetBSD: Makefile,v 1.16 2013/07/05 13:29:41 ryoon Exp $
#

DISTNAME=	choqok-1.3
PKGREVISION=	12
CATEGORIES=	net
MASTER_SITES=	${MASTER_SITE_SOURCEFORGE:=choqok/}Choqok/
EXTRACT_SUFX=	.tar.bz2

MAINTAINER=	jaapb@NetBSD.org
HOMEPAGE=	http://choqok.gnufolks.org/
COMMENT=	Twitter and StatusNet client for KDE
LICENSE=	gnu-gpl-v2

USE_LANGUAGES=	c c++
USE_TOOLS+=	perl msgfmt pkg-config

BUILD_DEPENDS+=         automoc4>=0.9.87:../../devel/automoc4
DEPENDS=	qca2-ossl-[0-9]*:../../security/qca2-ossl

.include "../../meta-pkgs/kde4/kde4.mk"
.include "../../x11/kdelibs4/buildlink3.mk"
.include "../../devel/qjson/buildlink3.mk"
.include "../../security/qca2/buildlink3.mk"
.include "../../security/qoauth/buildlink3.mk"
.include "../../misc/attica/buildlink3.mk"
.include "../../sysutils/desktop-file-utils/desktopdb.mk"
.include "../../mk/bsd.pkg.mk"
