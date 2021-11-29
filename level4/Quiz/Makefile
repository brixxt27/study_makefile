NAME := libft.a
SRCS := first.c \
	   second.c \
	   third.c
OBJS := $(SRCS:.c=.o)
AR := ar
ARFLAGS := -rcs

$(NAME) : $(OBJS)
	$(AR) $(ARFLAGS) $@ $<
%.o : %.c
	$(CC) $(CFLAGS) -c $<
