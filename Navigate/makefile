CC = gcc

CFLAGS = -Wall -std=c99 -O3

TARGET = navigate

SRCS = navigate.c builder.c processing.c navigation.c

HEADERS = navigate.h

OBJS = $(SRCS:.c=.o)

$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) -o $@ $(OBJS)

%.o: %.c $(HEADERS)
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJS) $(TARGET)
