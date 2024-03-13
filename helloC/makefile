CC = gcc
CFLAGS = -g -m64

PROG = hellw
SRC = hellw.c
OBJ = $(SRC:.c=.o)

all: clean $(PROG) test

%.o: %.c
	$(CC) $(CFLAGS) -c -o $@ $<

clean:
	rm -rf $(PROG) $(OBJ) $(COVIDIR)

$(PROG): $(OBJ)
	$(CC) $(CFLAGS) -o $@ $^

test: $(PROG)
	$(CURDIR)/$^
