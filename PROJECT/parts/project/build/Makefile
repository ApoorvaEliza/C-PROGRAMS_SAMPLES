# Usage:
# make        # compile all binary
# make clean  # remove ALL binaries and objects

.PHONY = all clean

CC = gcc                        # compiler to use

LINKERFLAG = -lm

SRCS := StuRec.c  IP_Validate.c
BINS := STU IPVAL

all: IPVAL STU
IPVAL: IPVAL.o
	@echo "Checking.."
	gcc -lm IPVAL.o -o IPVAL
STU: STU.o
	@echo "Checking.."
	gcc -lm STU.o -o STU


IPVAL.o: IP_Validate.c
	@echo "Creating object.."
	gcc -c IP_Validate.c -o IPVAL.o
STU.o: StuRec.c
	@echo "Creating object..."
	gcc -c StuRec.c -o STU.o


clean:
	@echo "Cleaning up..."
	rm -rvf IPVAL.o IPVAL STU.o STU
