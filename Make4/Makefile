#Usage:		

#make		#compile all binary

#make clean	#remove all binary and objects

.PHONY = all clean

CC = gcc

LINKERFLAG = -lm

SRCS := $(wildcard *.c)

BINS := $(SRCS:%.c=%)

all: ${BINS}

vowel: vowel.o
	@echo "Checking...."
	${CC} ${LINKERFLAG} vowel.o -o vowel 

vowel.o: vowel.c
	@echo "Creating...."
	${CC} -c vowel.c 

clean:
	@echo "Cleaning up...."
	rm -rvf vowel.o vowel 
