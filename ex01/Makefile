SOURCES=srcs/ft_putchar.c srcs/ft_putstr.c srcs/ft_strcmp.c srcs/ft_strlen.c srcs/ft_swap.c
OBJECTS=$(SOURCES:.c=.o)

%.o: %.c includes/ft.h
	gcc -Wall -Wextra -Werror -c $< -o $@

libft.a: $(OBJECTS)
	ar -cq libft.a $(OBJECTS)

clean:
	rm -f $(OBJECTS)

fclean: clean
	rm -f libft.a

all: libft.a

re: fclean all
