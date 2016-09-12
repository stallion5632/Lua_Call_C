CFLAGS= -I/usr/local/include -Wall  -fPIC
LIBS=-L/usr/local/lib -llua

all: test.so

test.o: test.c test.o
	$(CC) -c $< -o $@ ${CFLAGS}

test.so: test.o
	$(CC)  -o test.so test.o ${LIBS} --shared

clean:
	rm -rf *.so *.o
