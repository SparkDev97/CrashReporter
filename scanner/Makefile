TWEAK_NAME = scanner

scanner_INSTALL_PATH = /Applications/CrashReporter.app
scanner_FILES = \
	CRAlertItem.xm \
	CRCannotEmailAlertItem.xm \
	CRMailViewController.m \
	CRMissingFilterAlertItem.xm \
	Tweak.xm
scanner_FRAMEWORKS = MessageUI UIKit
scanner_LIBRARIES = packageinfo
scanner_CFLAGS = -Wno-deprecated-declarations

ARCHS = arm64 arm64e

include $(THEOS_MAKE_PATH)/common.mk
include $(THEOS_MAKE_PATH)/tweak.mk
