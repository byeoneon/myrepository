CC = gcc
CFLAGS = -g -Wall
OUTPUT = main
OBJFILE = player.o
.PHONY: clean

$(OUTPUT): $(OBJFILE)
	$(CC) -o $(OUTPUT) $(OBJFILE) -L../lib -lfuncs

%.o: %.c
	$(CC) $(CFLAGS) -I../include -c $< -o $@

clean:
	rm *.o $(OUTPUT)
