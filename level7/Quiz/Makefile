NAME = main

SRC = main.c
OBJ = $(SRC:.c=.o)
CSRCS = first.c \
		second.c \
		third.c
COBJS = $(CSRCS:.c=.o)
OBJS = $(SRCS:.c=.o)
LIBFT = libft.a
AR = ar
ARFLAGS = -rcs
CC = gcc
CFLAGS = -Wall -Wextra -Werror

all : $(NAME)

clean :
	rm -f *.o
fclean :
	rm -f $(NAME) $(LIBFT)
re : fclean all

$(NAME) : $(OBJ) $(LIBFT)
	$(CC) $(CFLAGS) -o $@ $?
$(LIBFT) : $(COBJS)
	$(AR) $(ARFLAGS) $@ $?
%.o : %.c
	$(CC) $(CFLAGS) -c $?

.PHONY : all clean fclean re
