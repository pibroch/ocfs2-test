TOPDIR = ../../../

include $(TOPDIR)/Preamble.make

TESTS = remove_slot

CFLAGS = -O2 -Wall -g

SOURCES = remove_slot.c
OBJECTS = $(patsubst %.c,%.o,$(SOURCES))

DIST_FILES = $(SOURCES) remove_slot.sh corrupt_remove_slot.sh

BIN_PROGRAMS = remove_slot

BIN_EXTRA = remove_slot.sh corrupt_remove_slot.sh

remove_slot: $(OBJECTS)
	$(LINK)  -locfs2 -lcom_err

include $(TOPDIR)/Postamble.make
