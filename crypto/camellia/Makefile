#
# crypto/camellia/Makefile
#

DIR= camellia
TOP=	../..
CC=	cc
CPP=	$(CC) -E
INCLUDES=
CFLAG=-g
MAKEFILE=	Makefile
AR=		ar r

CAMELLIA_ASM_OBJ=

CFLAGS= $(INCLUDES) $(CFLAG)
ASFLAGS= $(INCLUDES) $(ASFLAG)
AFLAGS= $(ASFLAGS)

GENERAL=Makefile
#TEST=camelliatest.c
APPS=

LIB=$(TOP)/libcrypto.a
LIBSRC=camellia.c cmll_misc.c cmll_ecb.c cmll_cbc.c cmll_ofb.c \
	   cmll_cfb.c cmll_ctr.c 

LIBOBJ= camellia.o cmll_misc.o cmll_ecb.o cmll_cbc.o cmll_ofb.o \
		cmll_cfb.o cmll_ctr.o $(CAMELLIA_ASM_OBJ)

SRC= $(LIBSRC)

EXHEADER= camellia.h
HEADER= cmll_locl.h $(EXHEADER)

ALL=    $(GENERAL) $(SRC) $(HEADER)

top:
	(cd ../..; $(MAKE) DIRS=crypto SDIRS=$(DIR) sub_all)

all:	lib

lib: lib_arx_common

$(LIBOBJ): $(LIBSRC)


files: files_common

links: links_up2_common

install: install_common

tags: tags_common

tests:

lint: lint_common

depend: depend_common

dclean: dclean_common

clean: clean_common clean_s_common

include $(TOP)/Makefile.common

# DO NOT DELETE THIS LINE -- make depend depends on it.

camellia.o: ../../include/openssl/e_os2.h ../../include/openssl/opensslconf.h
camellia.o: camellia.c camellia.h cmll_locl.h
cmll_cbc.o: ../../include/openssl/camellia.h ../../include/openssl/e_os2.h
cmll_cbc.o: ../../include/openssl/opensslconf.h cmll_cbc.c cmll_locl.h
cmll_cfb.o: ../../e_os.h ../../include/openssl/camellia.h
cmll_cfb.o: ../../include/openssl/e_os2.h ../../include/openssl/opensslconf.h
cmll_cfb.o: cmll_cfb.c cmll_locl.h
cmll_ctr.o: ../../include/openssl/camellia.h ../../include/openssl/e_os2.h
cmll_ctr.o: ../../include/openssl/opensslconf.h cmll_ctr.c cmll_locl.h
cmll_ecb.o: ../../include/openssl/camellia.h ../../include/openssl/e_os2.h
cmll_ecb.o: ../../include/openssl/opensslconf.h cmll_ecb.c cmll_locl.h
cmll_misc.o: ../../include/openssl/camellia.h ../../include/openssl/crypto.h
cmll_misc.o: ../../include/openssl/e_os2.h ../../include/openssl/fips.h
cmll_misc.o: ../../include/openssl/opensslconf.h
cmll_misc.o: ../../include/openssl/opensslv.h ../../include/openssl/ossl_typ.h
cmll_misc.o: ../../include/openssl/safestack.h ../../include/openssl/stack.h
cmll_misc.o: ../../include/openssl/symhacks.h cmll_locl.h cmll_misc.c
cmll_ofb.o: ../../include/openssl/camellia.h ../../include/openssl/e_os2.h
cmll_ofb.o: ../../include/openssl/opensslconf.h cmll_locl.h cmll_ofb.c
