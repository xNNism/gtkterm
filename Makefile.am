# GtkTerm Makefile.am

SUBDIRS = src po
man_MANS = gtkterm.1
EXTRA_DIST = TODO $(man_MANS)
desktopdir = $(datadir)/applications
desktop_in_files = gtkterm.desktop.in
desktop_DATA = $(desktop_in_files:.desktop.in=.desktop)

@INTLTOOL_DESKTOP_RULE@
