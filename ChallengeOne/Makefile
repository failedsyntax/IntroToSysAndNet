CC = gcc
CFLAGS = -Wall -pthread

SRCS = ThreadedMatrixMultiply.c
OBJS = $(SRCS:.c=.o)
TARGET = ThreadedMatrixMultiplication

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) $(OBJS) -o $(TARGET)  # <-- Make sure this uses a TAB

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@  # <-- Make sure this uses a TAB

clean:
	rm -f $(OBJS) $(TARGET)  # <-- Also ensure this uses a TAB
