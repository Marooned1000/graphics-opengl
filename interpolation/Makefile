UNAME_S := $(shell uname)

LDFLAGS += -lglut -lGL -lGLU -lGLEW -lGLU -lm -lGL -lglfw -lrt -lm -ldl

CPP = g++
CPP_FLAGS = -Wall
INC = -I/usr/include

all: main.exe

main.exe: main.o
	$(CPP) $^ -o $@ $(LDFLAGS)

main.o: main.cpp
	$(CPP) $(CPP_FLAGS) $(INC) -c $< -o $@

clean:
	rm -f *.o *.exe
