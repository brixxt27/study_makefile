NAME = libft.a
SRCS = first.c second.c third.c
OBJS = $(SRCS:.c=.o)
AR = ar
ARFLAGS = -rcs
CC = gcc
CFLAGS = -Wall -Wextra -Werror

all : $(NAME)

$(NAME) : $(OBJS)
	$(AR) $(ARFLAGS) $@ $<
%.o : %.c
	$(CC) $(CFLAGS) -c $<

clean :
	rm *.o
fclean :
	rm -f $(NAME)
re : fclean all

.PHONY : all clean fclean re
