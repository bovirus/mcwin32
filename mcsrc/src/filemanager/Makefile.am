
noinst_LTLIBRARIES = libmcfilemanager.la

libmcfilemanager_la_SOURCES = \
	achown.c \
	boxes.c boxes.h \
	cd.c cd.h \
	chmod.c \
	chown.c \
	cmd.c cmd.h \
	command.c command.h \
	dir.c dir.h \
	ext.c ext.h \
	file.c file.h \
	filegui.c filegui.h \
	filemanager.h filemanager.c \
	filenot.c filenot.h \
	find.c \
	hotlist.c hotlist.h \
	info.c info.h \
	ioblksize.h \
	layout.c layout.h \
	mountlist.c mountlist.h \
	panelize.c panelize.h \
	panel.c panel.h \
	tree.c tree.h \
	treestore.c treestore.h

# Unmaintained, unsupported, etc
#	listmode.c listmode.h

AM_CPPFLAGS = -I$(top_srcdir) $(GLIB_CFLAGS)

if ENABLE_EXT2FS_ATTR
libmcfilemanager_la_SOURCES += \
	chattr.c
endif
