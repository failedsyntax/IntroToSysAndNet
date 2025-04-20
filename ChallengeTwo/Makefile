CC = gcc
CFLAGS = -Wall -pthread

# Define both source files
SRCS := HTTP_Client.c HTTP_Server.c

# Create their .o files
OBJS := $(SRCS:.c=.o)

# Create both target files
TARGETS := $(SRCS:.c=)

.PHONY: all clean
all: $(TARGETS)

# For every target, if it's object file exists, then link it
$(TARGETS): %: %.o
	$(CC) $(CFLAGS) -o $@ $<

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJS) $(TARGETS)
