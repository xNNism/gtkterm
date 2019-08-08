# GtkTerm Makefile.am

SUBDIRS = src po
man_MANS = gtkterm.1
EXTRA_DIST = \
		TODO $(man_MANS) \
        gtkterm.desktop \
        gtkterm.png \
    autogen.sh

Applicationsdir = /usr/share/applications
Applications_DATA = gtkterm.desktop

#the application icon
appicondir=$(datadir)/icons/hicolor/scalable/apps
appicon_DATA=gtkterm.png

#icons in the application
NULL =

private_icons = \
	gtkterm.png\
  $(NULL)

install-icons:
	for icon in $(private_icons); do \
		mkdir -p $(DESTDIR)$(pkgdatadir)/icons/; \
		$(INSTALL_DATA) $(srcdir)/$$icon $(DESTDIR)$(pkgdatadir)/icons/; \
	done

install-data-local: install-icons
