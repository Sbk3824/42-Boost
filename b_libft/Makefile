# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: skuntoji <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2018/09/12 08:49:15 by skuntoji          #+#    #+#              #
#    Updated: 2018/09/13 00:18:05 by skuntoji         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME 	= libft.a

CFLAGS = -Wall -Werror -Wextra
FILES = ft_memset.c ft_strlen.c ft_strdup.c ft_strcpy.c ft_strncpy.c \
		ft_strchr.c  ft_strcmp.c ft_isdigit.c ft_toupper.c ft_tolower.c

OBJ = $(FILES:%.c=%.o)

all: $(NAME)

$(NAME): $(OBJ)
		ar rcs $(NAME) $(OBJ)

$(OBJ): $(FILES)
		gcc -c -I. $(CFLAGS) $(FILES)
clean:
		rm -f $(OBJ)
fclean: clean
		rm -f $(NAME)
re: fclean all
