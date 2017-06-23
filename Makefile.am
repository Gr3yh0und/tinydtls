include $(abs_top_nlbuild_autotools_dir)/automake/pre.am

EXTRA_DIST              = \
			  alert.h \
			  ccm.h \
			  crypto.h \
			  dtls.h \
			  dtls_config.h \
			  dtls_debug.h \
			  dtls_time.h \
			  global.h \
			  hmac.h \
			  netq.h \
			  numeric.h \
			  peer.h \
			  prng.h \
			  session.h \
			  state.h \
			  tinydtls.h \
			  uthash.h \
			  utlist.h \
			  aes/rijndael.h \
			  sha2/sha2.h \
			  $(NULL)

lib_LIBRARIES           = libtinydtls.a

libtinydtls_a_CPPFLAGS = \
			 -I$(top_srcdir)/third_party/tinydtls \
			 -I$(top_srcdir)/include              \
			 -I$(top_srcdir)/include/openthread   \
			 -I$(top_srcdir)/include/openthread/platform \
			 -DHAVE_ASSERT_H                      \
			 -DDTLS_PEERS_NOHASH                  \
			 -DSHA2_USE_INITTYPES_H               \
			 -DWITH_SHA256                        \
			 -DHAVE_SYS_TIME_H                    \
			 -DHAVE_VPRINTF                       \
			 $(CPPFLAGS)                          \
			 $(NULL)

libtinydtls_a_SOURCES  = \
			 ccm.c \
			 crypto.c \
			 dtls.c \
			 dtls_debug.c \
			 dtls_time.c \
			 hmac.c \
			 netq.c \
			 peer.c \
			 session.c \
			 aes/rijndael.c \
			 sha2/sha2.c \
			 $(NULL)

noinst_HEADERS          =  \
			   alert.h \
			   ccm.h \
			   crypto.h \
			   dtls.h \
			   dtls_config.h \
			   dtls_debug.h \
			   dtls_time.h \
			   global.h \
			   hmac.h \
			   netq.h \
			   numeric.h \
			   peer.h \
			   prng.h \
			   session.h \
			   state.h \
			   tinydtls.h \
			   uthash.h \
			   utlist.h \
			   aes/rijndael.h \
			   sha2/sha2.h \
			   $(NULL)

include $(abs_top_nlbuild_autotools_dir)/automake/post.am
