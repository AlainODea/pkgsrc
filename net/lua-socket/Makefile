# $NetBSD: Makefile,v 1.5 2013/09/13 14:24:28 fhajny Exp $
#

DISTNAME=		luasocket-3.0-rc1
PKGNAME=		${LUA_PKGPREFIX}-${DISTNAME:S/lua//:S/-rc/rc/}
PKGREVISION=		1
CATEGORIES=		net
MASTER_SITES=		-https://github.com/diegonehab/luasocket/archive/v3.0-rc1.tar.gz

MAINTAINER=		pkgsrc-users@NetBSD.org
HOMEPAGE=		http://w3.impa.br/~diego/software/luasocket/
COMMENT=		Network support for the Lua language
LICENSE=		mit

FETCH_USING=		curl

MAKE_FILE=		makefile

LDFLAGS.SunOS=		-lrt -lresolv

MAKE_FLAGS+=		LUAV=5.2
MAKE_FLAGS+=		LUAINC_linux_base=${PREFIX}/include
MAKE_FLAGS+=		LUAPREFIX_linux=${PREFIX}

.include "../../lang/lua/module.mk"
.include "../../mk/bsd.pkg.mk"
