CC=gcc 

CPPFLAGS= -MMD `pkg-config --cflags SDL2_image` 
CFLAGS= -Wall -Wextra -std=c99 -O3 -g -lm -ldl -lSDL2 -lSDL2_image -D__NO_INLINE__
LDFLAGS= 
LDLIBS= `pkg-config --libs sdl SDL2_image`
SCR = rotation.c main.c  
OBJ = $(SCR:%.c = %.o)
all: main

main: $(OBJ)
	gcc  $(CFLAGS) -o $@ $^

clean:
    ${RM} ${OBJ} 
    ${RM} main
