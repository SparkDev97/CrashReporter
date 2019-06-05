TARGET = iphone:latest:7.0
ARCHS = arm64 arm64e

SDKVERSION = 11.2
SYSROOT = $(THEOS)/sdks/iPhoneOS11.2.sdk

TOOL_NAME = notifier
notifier_INSTALL_PATH = /Applications/CrashReporter.app
notifier_FILES = \
    ../common/crashlog_util.m \
    ../common/exec_as_root.m \
    main.m
notifier_LDFLAGS = -lcrashreport
notifier_PRIVATE_FRAMEWORKS = SpringBoardServices
notifier_CODESIGN_FLAGS="-SEntitlements.plist"
notifier_CFLAGS = -Wno-deprecated-declarations

include $(THEOS_MAKE_PATH)/common.mk
include $(THEOS_MAKE_PATH)/tool.mk

after-clean::
	- rm -rf $(THEOS_PROJECT_DIR)/notifier/Common
	- rm -rf $(THEOS_PROJECT_DIR)/notifier/common
