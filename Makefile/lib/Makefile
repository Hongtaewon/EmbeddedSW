AR = ar
CC = gcc
CFLAGS = -g -Wall -I../include
OUTPUT = libfuncs.a
SRCS = func1.c func2.c
OBJFILES = func1.o func2.o
.PHONY : clean

$(OUTPUT) : $(OBJFILES)
	$(AR) rv $(OUTPUT) $(OBJFILES)

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJFILES) $(OUTPUT)
