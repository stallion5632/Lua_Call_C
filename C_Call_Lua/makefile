CFLAGS= -I/usr/local/include  -Wall 
LIBS=-L/usr/local/lib -llua

all: test

test.o: test.c test.o
	$(CC) -c $< -o $@ ${CFLAGS}

test: test.o
	$(CC)  -o test test.o ${LIBS} 

clean:
	rm -rf test *.o
