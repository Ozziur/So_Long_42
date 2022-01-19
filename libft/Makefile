
# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: mruizzo <marvin@42.fr>                     +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/01/10 13:00:01 by mruizzo           #+#    #+#              #
#    Updated: 2022/01/10 15:52:29 by mruizzo          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

CC = gcc
FLAGS = -Wall -Wextra -Werror

NAME = libft.a
SRC = ft_isprint.c ft_memcmp.c ft_atoi.c ft_strlcat.c ft_strncmp.c ft_isalpha.c ft_memcpy.c \
		ft_strchr.c  ft_strlcpy.c ft_tolower.c ft_bzero.c ft_isascii.c ft_isalnum.c \
		ft_memmove.c ft_strlen.c  ft_strrchr.c ft_calloc.c ft_strdup.c ft_toupper.c \
		ft_isdigit.c ft_memchr.c ft_memset.c ft_strnstr.c ft_substr.c ft_strjoin.c \
		ft_strtrim.c ft_split.c ft_itoa.c ft_strmapi.c ft_striteri.c ft_putchar_fd.c \
		ft_putstr_fd.c ft_putendl_fd.c ft_putnbr_fd.c

BONUS = ft_lstnew.c ft_lstadd_front.c ft_lstsize.c ft_lstlast.c ft_lstadd_back.c \
		ft_lstdelone.c ft_lstclear.c ft_lstiter.c ft_lstmap.c

OBJ = $(SRC:.c=.o)
B_OBJ = $(BONUS:.c=.o)

%.o: %.c
	$(CC) $(FLAGS) -c $< -o $@

all: $(NAME)

$(NAME): $(OBJ)
	ar -rc $(NAME) $(OBJ)

bonus: $(OBJ) $(B_OBJ)
	ar -rc $(NAME) $(OBJ) $(B_OBJ)

clean:
	rm -f $(OBJ) $(B_OBJ)

fclean: clean
	rm -f $(NAME)

re: fclean all

.PHONY: all clean fclean re bonus
