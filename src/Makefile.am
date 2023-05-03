bin_PROGRAMS = startupwiz \
			   startupwizhs

dist_bin_SCRIPTS = hdmi-audio-select

startupwiz_CFLAGS = \
	-I$(top_srcdir) \
	-DPACKAGE_LIB_DIR=\""$(libdir)"\" \
	-DPACKAGE_DATA_DIR=\""$(datadir)/startupwiz"\" \
	-DPACKAGE_UI_DIR=\""$(datadir)/startupwiz/ui"\" \
	-DPACKAGE_BIN_DIR=\""$(bindir)"\" \
	-DPACKAGE_LOCALE_DIR=\""$(prefix)/$(DATADIRNAME)/locale"\" \
	-I$(srcdir)/libdhcpcd \
	-I$(srcdir)/dhcpcd-gtk \
	$(PACKAGE_CFLAGS) \
	$(G_CAST_CHECKS) \
	-Wall

startupwiz_SOURCES = startup-wiz.c \
		libdhcpcd/config.c \
		libdhcpcd/dhcpcd.c \
		libdhcpcd/wpa.c \
		dhcpcd-gtk/wpa.c \
		dhcpcd-gtk/main.c

startupwiz_includedir = $(includedir)/startupwiz

startupwiz_include_HEADERS =

startupwiz_LDFLAGS = $(DYNAMIC_FLAGS) -lcrypt
startupwiz_DEPENDENCIES_EXTRA = $(BUILTIN_PLUGINS)

startupwiz_LDADD = \
		$(BUILTIN_PLUGINS) \
		$(PACKAGE_LIBS) \
		$(X11_LIBS) \
		$(INTLLIBS)

startupwizhs_CFLAGS = \
	-I$(top_srcdir) \
	-DPACKAGE_LIB_DIR=\""$(libdir)"\" \
	-DPACKAGE_DATA_DIR=\""$(datadir)/startupwiz"\" \
	-DPACKAGE_UI_DIR=\""$(datadir)/startupwiz/ui"\" \
	-DPACKAGE_BIN_DIR=\""$(bindir)"\" \
	-DPACKAGE_LOCALE_DIR=\""$(prefix)/$(DATADIRNAME)/locale"\" \
	-DHOMESCHOOL \
	-I$(srcdir)/libdhcpcd \
	-I$(srcdir)/dhcpcd-gtk \
	$(PACKAGE_CFLAGS) \
	$(G_CAST_CHECKS) \
	-Wall

startupwizhs_SOURCES = startup-wiz.c \
		libdhcpcd/config.c \
		libdhcpcd/dhcpcd.c \
		libdhcpcd/wpa.c \
		dhcpcd-gtk/wpa.c \
		dhcpcd-gtk/main.c

startupwizhs_includedir = $(includedir)/startupwiz

startupwizhs_include_HEADERS =

startupwizhs_LDFLAGS = $(DYNAMIC_FLAGS) -lcrypt
startupwizhs_DEPENDENCIES_EXTRA = $(BUILTIN_PLUGINS)

startupwizhs_LDADD = \
		$(BUILTIN_PLUGINS) \
		$(PACKAGE_LIBS) \
		$(X11_LIBS) \
		$(INTLLIBS)
		
EXTRA_DIST =
