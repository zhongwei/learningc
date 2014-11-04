ROOT=..
PLATFORM=$(shell $(ROOT)/systype.sh)
include $(ROOT)/Make.defines.$(PLATFORM)

PROGS =	hello_world hello_world2 f2c f2c_float f2c_for f2c_define \
		getput_char getput_char2 count_chars count_chars_for \
		count_lines count_words power array_test array_chars var_scope

all:	$(PROGS)

%:	%.c
	$(CC) $(CFLAGS) $@.c -o $@ $(LDFLAGS)

clean:
	rm -f $(PROGS) $(TEMPFILES) *.o

