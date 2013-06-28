glib_enum_prefix = gst_dts

include glib-gen.mak

# plugindir is set in configure

EXTRA_DIST = gstdts-marshal.list

plugin_LTLIBRARIES = libgstdtsdownmix.la

# for the next set of variables, rename the prefix if you renamed the .la

# sources used to compile this plug-in
libgstdtsdownmix_la_SOURCES = gstdtsdownmix.c

# flags used to compile this plugin
# add other _CFLAGS and _LIBS as needed
libgstdtsdownmix_la_CFLAGS = $(GST_CFLAGS)
libgstdtsdownmix_la_LIBADD = $(GST_LIBS) -lgstbase-$(GST_MAJORMINOR) $(DTS_LIBS)
libgstdtsdownmix_la_LDFLAGS = $(GST_PLUGIN_LDFLAGS)

# headers we need but don't want installed
noinst_HEADERS = gstdtsdownmix.h

