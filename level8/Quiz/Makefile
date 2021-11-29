NAME = main

SRC_DIR = ./src/
SRC_NAME = main.c \
		   first.c \
		   second.c \
		   third.c
SRC = $(addprefix $(SRC_DIR),$(SRC_NAME))

OBJ_DIR = ./obj/
OBJ_NAME = $(SRC_NAME:.c=.o)
OBJ = $(addprefix $(OBJ_DIR),$(OBJ_NAME))

AR = ar
ARFLAGS = -rcs
CC = gcc
CFLAGS = -Wall -Wextra -Werror
INCLUDE = -I./include

$(NAME) : $(OBJS) $(LIBFT)

%.o : %.c :
	$(CC) $(CFLAGS) -c $(SRC)
