# $OpenBSD: Makefile,v 1.1.1.1 2018/12/19 07:45:47 rsadowski Exp $

COMMENT =	certificate manager and a universal crypto GUI
DISTNAME =	kleopatra-${VERSION}
CATEGORIES =	security x11

SHARED_LIBS +=  kleopatraclientcore       0.0 # 1.3
SHARED_LIBS +=  kleopatraclientgui        0.0 # 1.3

KDE5 =		Yes

WANTLIB += ${COMPILER_LIBCXX} KF5Auth KF5Codecs KF5ConfigCore
WANTLIB += KF5ConfigGui KF5ConfigWidgets KF5CoreAddons KF5Crash
WANTLIB += KF5DBusAddons KF5I18n KF5IconThemes KF5ItemModels KF5KCMUtils
WANTLIB += KF5Mime KF5Notifications KF5Service KF5SonnetUi KF5TextWidgets
WANTLIB += KF5WidgetsAddons KF5WindowSystem KF5XmlGui Qt5Core
WANTLIB += Qt5DBus Qt5Gui Qt5Network Qt5PrintSupport Qt5Widgets
WANTLIB += Qt5Xml assuan c gpg-error gpgmepp m qgpgme

MODKDE5_DESKTOP_FILE = yes
MODKDE5_ICON_CACHE = yes
MODKDE5_TRANSLATIONS = yes
MODKDE5_DOCS = yes

MODULES +=	x11/kde-applications

LIB_DEPENDS +=	devel/kf5/kauth \
		devel/kf5/kcmutils \
		devel/kf5/kcodecs \
		devel/kf5/kconfig \
		devel/kf5/kconfigwidgets \
		devel/kf5/kcoreaddons \
		devel/kf5/kcrash \
		devel/kf5/kdbusaddons \
		devel/kf5/ki18n \
		devel/kf5/kiconthemes \
		devel/kf5/kitemmodels \
		devel/kf5/knotifications \
		devel/kf5/kservice \
		devel/kf5/ktextwidgets \
		devel/kf5/kwidgetsaddons \
		devel/kf5/kwindowsystem \
		devel/kf5/kxmlgui \
		devel/kf5/sonnet \
		security/gpgme,-qt \
		security/libassuan \
		security/libgpg-error \
		x11/kde-applications/kmime

.include <bsd.port.mk>
