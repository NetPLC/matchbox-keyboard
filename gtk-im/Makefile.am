AM_CFLAGS = -Wall

if WANT_GTK2_IM
gtk2imdir = @libdir@/gtk-2.0/@GTK_VERSION@/immodules/
gtk2im_LTLIBRARIES = libmbgtk2-im-invoker.la
# TODO: remove lib prefix

libmbgtk2_im_invoker_la_CPPFLAGS = @GTK2_CFLAGS@ -I${top_srcdir}/src
libmbgtk2_im_invoker_la_LDFLAGS = -avoid-version
libmbgtk2_im_invoker_la_LIBADD = @GTK2_LIBS@

libmbgtk2_im_invoker_la_SOURCES = \
        im-module.c \
        im-context.h im-context.c \
        im-protocol.h im-protocol.c
endif

if WANT_GTK3_IM
gtk3imdir = @libdir@/gtk-3.0/@GTK3VERSION@/immodules/
gtk3im_LTLIBRARIES = libmbgtk3-im-invoker.la
# TODO: remove lib prefix

libmbgtk3_im_invoker_la_CPPFLAGS = @GTK3_CFLAGS@ -I${top_srcdir}/src
libmbgtk3_im_invoker_la_LDFLAGS = -avoid-version
libmbgtk3_im_invoker_la_LIBADD = @GTK3_LIBS@

libmbgtk3_im_invoker_la_SOURCES = \
	im-module.c \
	im-context.h im-context.c \
	im-protocol.h im-protocol.c
endif
