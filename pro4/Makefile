CC=gcc
CFLAGS=-Wall -g

TARGET=ex4
SRCS=$(wildcard *.c)
OBJS=$(patsubst &.c,%.o,$(SRCS))

all:$(TARGET)

$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) -o $@ $^

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJS) $(TARGET)
