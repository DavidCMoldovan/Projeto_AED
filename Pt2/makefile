CC = gcc

ifdef DEBUG
MODE = -g
else
MODE = -O3
endif

CFLAGS = -Wall -std=c99 $(MODE) 

TARGET = navigate

SRCS = navigate.c graph.c stack.c

HEADERS = navigate.h stack.h

OBJS = $(SRCS:.c=.o)

$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) -o $@ $(OBJS)

%.o: %.c $(HEADERS)
	$(CC) $(CFLAGS) -c $< -o $@
  
clean:
	rm -f *.o $(TARGET)
