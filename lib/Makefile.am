lib_LTLIBRARIES = libfw_env.la
libfw_env_la_SOURCES = ctype.c linux_string.c crc32.c env_attr.c env_flags.c fw_env.c
libfw_env_la_CFLAGS = -Wall -Wextra -g -DUSE_HOSTCC
libfw_env_la_CFLAGS +=  -I$(top_srcdir)/include/
libfw_env_la_LDFLAGS = -version-number $(subst .,:,$(VERSION_CODE))
