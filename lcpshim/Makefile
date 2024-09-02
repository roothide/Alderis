include $(THEOS)/makefiles/common.mk

LIBRARY_NAME = libcolorpicker

libcolorpicker_FILES = $(wildcard *.m)
libcolorpicker_PRIVATE_FRAMEWORKS = Preferences
libcolorpicker_INSTALL_PATH = $(THEOS_PACKAGE_INSTALL_PREFIX)/usr/lib
ifeq ($(ROOTHIDE),1)
libcolorpicker_LDFLAGS = -install_name @loader_path/.jbroot/usr/lib/libcolorpicker.dylib
else
libcolorpicker_LDFLAGS = -install_name @rpath/libcolorpicker.dylib
endif

include $(THEOS_MAKE_PATH)/library.mk
