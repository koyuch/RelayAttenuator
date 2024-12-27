S_PATH=../..

AUTOMAKE_OPTIONS = subdir-objects

bin_PROGRAMS = r_attenu r_attenuc

AM_CXXFLAGS = $(INTI_CFLAGS)

r_attenu_SOURCES = r_attenu.c \
		$(S_PATH)/lib/config_file.c $(S_PATH)/lib/config_file.h \
		$(S_PATH)/lib/dump_config.c $(S_PATH)/lib/dump_config.h \
		$(S_PATH)/lib/input_map.c $(S_PATH)/lib/input_map.h \
		$(S_PATH)/lib/transmit.c $(S_PATH)/lib/transmit.h

r_attenu_CFLAGS = -I$(S_PATH) -I$(S_PATH)/lib -I$(S_PATH)/include -lwiringPi -llirc_client -lm -O0
r_attenu_LDFLAGS = -L$(S_PATH)/lib
r_attenu_LDADD = -llirc

r_attenuc_SOURCES = r_attenuc.c

