CFLAGS = -Wall -std=c99 -g
LDFLAGS = -lm -pthread -L$(HOME)/local/lib -lSDL
LIBFILE = libfractal/libfractal.a

main : main.o $(LIBFILE)
	@gcc -o main main.o $(LIBFILE) $(LDFLAGS)

main.o : main.c
	@gcc -c $(CFLAGS) main.c

$(LIBFILE) :
	@cd libfractal && make

lib :
	@cd libfractal && make

clean :
	@rm main main.o
	@cd libfractal && make clean


