# Usage:
# make        # compile all binary
# make clean  # remove ALL binaries and objects

.PHONY = all clean

CC = gcc                        # compiler to use

LINKERFLAG = -lm

SRCS := StuRec.c  IP_Validate.c
BINS := STU IPVAL

all: CHECKPING

CHECKPING: CHECKPING.o
	@echo "Checking.."
	gcc -lm CHECKPING.o -o CHECKPING



CHECKPING.o: ping.c
	@echo "Creating object..."
	gcc -c ping.c -o CHECKPING.o


clean:
	@echo "Cleaning up..."
	rm -rvf CHECKPING.o CHECKPING 
