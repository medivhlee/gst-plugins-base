if HAVE_GTK_X11
if HAVE_LINUX_JOYSTICK_HEADERS
GTK_EXAMPLES=seek scrubby jsseek
else
GTK_EXAMPLES=seek scrubby
endif
endif

examples = $(GTK_EXAMPLES) stepping stepping2

noinst_PROGRAMS = $(examples)

LDADD = \
	$(top_builddir)/gst-libs/gst/interfaces/libgstinterfaces-@GST_MAJORMINOR@.la \
	$(GST_LIBS) $(GTK_LIBS) $(LIBM)

AM_CFLAGS = -I$(top_builddir)/gst-libs $(GST_PLUGINS_BASE_CFLAGS) $(GST_BASE_CFLAGS) $(GST_CFLAGS) $(GTK_CFLAGS)
