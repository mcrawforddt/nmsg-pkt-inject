#CC = gcc --std=gnu99
AM_CFLAGS = -fstack-protector --param=ssp-buffer-size=4 -Wformat -Werror=format-security -O3 -ggdb -Wall -Wno-strict-aliasing -pthread -D_REENTRANT
AM_LDFLAGS = -Wl,-z,relro -lpthread -lpcap -lnmsg

BINS = nmsg-pkt-inject
bin_PROGRAMS = nmsg-pkt-inject

all: $(BINS)

NMSG_PKT_INJECT_OBJS = \
	argv.o \
	nmsg-pkt-inject.o

.PHONY: all clean
