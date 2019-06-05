TARGET = iphone:latest:7.0
ARCHS = arm64 arm64e

SDKVERSION = 11.2
SYSROOT = $(THEOS)/sdks/iPhoneOS11.2.sdk

TWEAK_NAME = monitor
monitor_INSTALL_PATH = /Applications/CrashReporter.app
monitor_FILES = Tweak.xm
monitor_PRIVATE_FRAMEWORKS = SpringBoardServices

ARCHS = arm64 arm64e

include $(THEOS_MAKE_PATH)/common.mk
include $(THEOS_MAKE_PATH)/tweak.mk
