#
# OpenSSL/fips/dh/Makefile
#

DIR=	dh
TOP=	../..
CC=	cc
INCLUDES=
CFLAG=-g
INSTALL_PREFIX=
OPENSSLDIR=     /usr/local/ssl
INSTALLTOP=/usr/local/ssl
MAKEDEPPROG=	makedepend
MAKEDEPEND=	$(TOP)/util/domd $(TOP) -MD $(MAKEDEPPROG)
MAKEFILE=	Makefile
AR=		ar r

CFLAGS= $(INCLUDES) $(CFLAG)

GENERAL=Makefile
TEST=
APPS=

LIB=$(TOP)/libcrypto.a
LIBSRC=fips_dh_check.c fips_dh_gen.c fips_dh_key.c fips_dh_lib.c
LIBOBJ=fips_dh_check.o fips_dh_gen.o fips_dh_key.o fips_dh_lib.o

SRC= $(LIBSRC)

EXHEADER=
HEADER=	$(EXHEADER)

ALL=    $(GENERAL) $(SRC) $(HEADER)

top:
	(cd $(TOP); $(MAKE) DIRS=fips FDIRS=$(DIR) sub_all)

all:	lib

lib:	$(LIBOBJ)
	@echo $(LIBOBJ) > lib

files: files_common

links: links_top_common

install: install_fips_common

tags: tags_common

tests:

fips_test:

lint: lint_common

depend:
	$(MAKEDEPEND) -- $(CFLAG) $(INCLUDES) $(DEPFLAG) -- $(SRC) $(TEST)

dclean: dclean_common

clean: clean_common

include $(TOP)/Makefile.common

# DO NOT DELETE THIS LINE -- make depend depends on it.

fips_dh_check.o: ../../include/openssl/bio.h ../../include/openssl/bn.h
fips_dh_check.o: ../../include/openssl/crypto.h ../../include/openssl/dh.h
fips_dh_check.o: ../../include/openssl/e_os2.h ../../include/openssl/err.h
fips_dh_check.o: ../../include/openssl/fips.h ../../include/openssl/lhash.h
fips_dh_check.o: ../../include/openssl/opensslconf.h
fips_dh_check.o: ../../include/openssl/opensslv.h
fips_dh_check.o: ../../include/openssl/ossl_typ.h
fips_dh_check.o: ../../include/openssl/safestack.h
fips_dh_check.o: ../../include/openssl/stack.h ../../include/openssl/symhacks.h
fips_dh_check.o: fips_dh_check.c
fips_dh_gen.o: ../../include/openssl/bio.h ../../include/openssl/bn.h
fips_dh_gen.o: ../../include/openssl/crypto.h ../../include/openssl/dh.h
fips_dh_gen.o: ../../include/openssl/e_os2.h ../../include/openssl/err.h
fips_dh_gen.o: ../../include/openssl/fips.h ../../include/openssl/lhash.h
fips_dh_gen.o: ../../include/openssl/opensslconf.h
fips_dh_gen.o: ../../include/openssl/opensslv.h
fips_dh_gen.o: ../../include/openssl/ossl_typ.h
fips_dh_gen.o: ../../include/openssl/safestack.h ../../include/openssl/stack.h
fips_dh_gen.o: ../../include/openssl/symhacks.h fips_dh_gen.c
fips_dh_key.o: ../../include/openssl/bio.h ../../include/openssl/bn.h
fips_dh_key.o: ../../include/openssl/crypto.h ../../include/openssl/dh.h
fips_dh_key.o: ../../include/openssl/e_os2.h ../../include/openssl/err.h
fips_dh_key.o: ../../include/openssl/fips.h ../../include/openssl/lhash.h
fips_dh_key.o: ../../include/openssl/opensslconf.h
fips_dh_key.o: ../../include/openssl/opensslv.h
fips_dh_key.o: ../../include/openssl/ossl_typ.h ../../include/openssl/rand.h
fips_dh_key.o: ../../include/openssl/safestack.h ../../include/openssl/stack.h
fips_dh_key.o: ../../include/openssl/symhacks.h fips_dh_key.c
fips_dh_lib.o: ../../include/openssl/bio.h ../../include/openssl/bn.h
fips_dh_lib.o: ../../include/openssl/crypto.h ../../include/openssl/dh.h
fips_dh_lib.o: ../../include/openssl/e_os2.h
fips_dh_lib.o: ../../include/openssl/opensslconf.h
fips_dh_lib.o: ../../include/openssl/opensslv.h
fips_dh_lib.o: ../../include/openssl/ossl_typ.h
fips_dh_lib.o: ../../include/openssl/safestack.h ../../include/openssl/stack.h
fips_dh_lib.o: ../../include/openssl/symhacks.h fips_dh_lib.c
