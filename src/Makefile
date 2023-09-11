MPICC=mpicxx
#CCFLAGS=-O3 -DDEBUG
CCFLAGS=-O3 -DDEBUG
LDFLAGS=-lm -O3

all: tsp-mpi

tsp-mpi: tsp-mpi.o
        $(MPICC) -o tsp-mpi tsp-mpi.o $(LDFLAGS)

tsp-mpi.o : tsp-mpi.c
        $(MPICC) -o tsp-mpi.o -c tsp-mpi.c $(CCFLAGS)

clean:
        rm tsp-mpi tsp-mpi.o

