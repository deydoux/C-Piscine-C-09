SOURCES=srcs/ft_putchar.c srcs/ft_putstr.c srcs/ft_strcmp.c srcs/ft_strlen.c srcs/ft_swap.c
OBJECTS=$(SOURCES:.c=.o)

all: libft.a

libft.a: $(OBJECTS)
	ar -cq libft.a $(OBJECTS)

%.o: %.c includes/ft.h
	gcc -Wall -Wextra -Werror -c $< -o $@

clean:
	rm -f $(OBJECTS)

fclean: clean
	rm -f libft.a

re: fclean all
