# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: bsouchet <bsouchet@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2016/02/02 15:48:09 by bsouchet          #+#    #+#              #
#    Updated: 2016/02/04 14:15:34 by bsouchet         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libft.a

HEADER = includes

SRC = ft_bzero.c \
	  ft_strcat.c \
	  ft_strcpy.c \
	  ft_memset.c \
	  ft_strlen.c \
	  ft_strnew.c \
	  ft_strjoin.c \
	  ft_memalloc.c

OBJ = $(SRC:.c=.o)

$(NAME):
	@gcc -Wall -Wextra -Werror -c $(SRC) -I $(HEADER)
	@ar rc $(NAME) $(OBJ)
	@ranlib $(NAME)

all: $(NAME)

clean:
	@rm -f $(OBJ)

fclean: clean
	@rm -f $(NAME)

re: fclean all
