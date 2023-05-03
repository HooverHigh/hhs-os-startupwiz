bin_PROGRAMS = startup-wiz \
			   startup-wizhs

dist_bin_SCRIPTS = hdmi-audio-select

startup-wiz_CFLAGS = \
	-I$(top_srcdir) \
	-DPACKAGE_LIB_DIR=\""$(libdir)"\" \
	-DPACKAGE_DATA_DIR=\""$(datadir)/startup-wiz"\" \
	-DPACKAGE_UI_DIR=\""$(datadir)/startup-wiz/ui"\" \
	-DPACKAGE_BIN_DIR=\""$(bindir)"\" \
	-DPACKAGE_LOCALE_DIR=\""$(prefix)/$(DATADIRNAME)/locale"\" \
	-I$(srcdir)/libdhcpcd \
	-I$(srcdir)/dhcpcd-gtk \
	$(PACKAGE_CFLAGS) \
	$(G_CAST_CHECKS) \
	-Wall

startup-wiz_SOURCES = startup-wiz.c \
		libdhcpcd/config.c \
		libdhcpcd/dhcpcd.c \
		libdhcpcd/wpa.c \
		dhcpcd-gtk/wpa.c \
		dhcpcd-gtk/main.c

startup-wiz_includedir = $(includedir)/startup-wiz

startup-wiz_include_HEADERS =

startup-wiz_LDFLAGS = $(DYNAMIC_FLAGS) -lcrypt
startup-wiz_DEPENDENCIES_EXTRA = $(BUILTIN_PLUGINS)

startup-wiz_LDADD = \
		$(BUILTIN_PLUGINS) \
		$(PACKAGE_LIBS) \
		$(X11_LIBS) \
		$(INTLLIBS)

startup-wizhs_CFLAGS = \
	-I$(top_srcdir) \
	-DPACKAGE_LIB_DIR=\""$(libdir)"\" \
	-DPACKAGE_DATA_DIR=\""$(datadir)/startup-wiz"\" \
	-DPACKAGE_UI_DIR=\""$(datadir)/startup-wiz/ui"\" \
	-DPACKAGE_BIN_DIR=\""$(bindir)"\" \
	-DPACKAGE_LOCALE_DIR=\""$(prefix)/$(DATADIRNAME)/locale"\" \
	-DHOMESCHOOL \
	-I$(srcdir)/libdhcpcd \
	-I$(srcdir)/dhcpcd-gtk \
	$(PACKAGE_CFLAGS) \
	$(G_CAST_CHECKS) \
	-Wall

startup-wizhs_SOURCES = startup-wiz.c \
		libdhcpcd/config.c \
		libdhcpcd/dhcpcd.c \
		libdhcpcd/wpa.c \
		dhcpcd-gtk/wpa.c \
		dhcpcd-gtk/main.c

startup-wizhs_includedir = $(includedir)/startup-wiz

startup-wizhs_include_HEADERS =

startup-wizhs_LDFLAGS = $(DYNAMIC_FLAGS) -lcrypt
startup-wizhs_DEPENDENCIES_EXTRA = $(BUILTIN_PLUGINS)

startup-wizhs_LDADD = \
		$(BUILTIN_PLUGINS) \
		$(PACKAGE_LIBS) \
		$(X11_LIBS) \
		$(INTLLIBS)
		
EXTRA_DIST =
