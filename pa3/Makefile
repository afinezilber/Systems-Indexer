CFLAGS = -Wall -g

all: index

index: tokens.o traverse.o index.o main.o
	gcc $(CFLAGS) tokens.o traverse.o index.o main.o -o index

tokens.o: tokens.c
	gcc $(CFLAGS) -c tokens.c -o tokens.o

traverse.o: traverse.c
	gcc $(CFLAGS) -c traverse.c -o traverse.o

index.o: index.c
	gcc $(CFLAGS) -c index.c -o index.o

main.o: main.c
	gcc $(GFLAGS) -c main.c -o main.o

clean:
	rm -f index
	rm -f *.o
