all: exec

exec: test.o sum.o
	gcc -o exec test.c sum.c

test.o: test.c
	gcc -c test.c

sum.o: sum.c
	gcc -c sum.c

.PHONY: clean

clean:
	rm exec *.o
