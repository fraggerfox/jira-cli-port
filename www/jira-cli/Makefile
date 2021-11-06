# WIP Package, remove / replace all wip instances before submission

PORTNAME=	jira-cli
DISTVERSIONPREFIX=	v
DISTVERSION=	0.1.1
CATEGORIES=	wip www
DIST_SUBDIR=	jira-cli

MAINTAINER=	fox@FreeBSD.org
COMMENT=	Feature-rich Interactive Jira Command Line

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=		go:modules

GO_MODULE=	github.com/ankitpokhrel/jira-cli
GO_TARGET=	./cmd/jira

post-install:
	${STAGEDIR}${PREFIX}/bin/jira man -g -o ${STAGEDIR}${MANPREFIX}/man/man7

.include <bsd.port.mk>
