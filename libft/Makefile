# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: eabdelha <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2021/11/06 18:21:52 by eabdelha          #+#    #+#              #
#    Updated: 2021/11/13 08:42:06 by eabdelha         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #
NAME = libft.a

FOBJ_LIBFT = ../object_files/object_files_libft
OBJECT_PATH = ../object_files/object_files_libft/

CC = gcc

CFLAGS = -Wall -Wextra -Werror

SRC =   ft_memset.c     \
		ft_bzero.c      \
		ft_memcpy.c     \
		ft_memmove.c    \
		ft_memchr.c     \
		ft_memcmp.c     \
		ft_strlen.c     \
		ft_isalpha.c    \
		ft_isdigit.c    \
		ft_isalnum.c    \
		ft_isascii.c    \
		ft_isprint.c    \
		ft_toupper.c    \
		ft_tolower.c    \
		ft_strchr.c     \
		ft_strrchr.c    \
		ft_strncmp.c    \
		ft_strlcpy.c    \
		ft_strlcat.c    \
		ft_strnstr.c    \
		ft_atoi.c       \
		ft_calloc.c		\
		ft_strdup.c		\
		ft_substr.c		\
		ft_strjoin.c	\
		ft_strtrim.c	\
		ft_putchar_fd.c	\
		ft_putstr_fd.c	\
		ft_putendl_fd.c	\
		ft_putnbr_fd.c	\
		ft_split.c		\
		ft_itoa.c		\
		ft_strmapi.c	\
		ft_striteri.c 	\
        ft_lstnew.c		\
		ft_lstadd_front.c \
		ft_lstsize.c	\
		ft_lstlast.c	\
		ft_lstadd_back.c \
		ft_lstdelone.c	\
		ft_lstclear.c	\
		ft_lstiter.c	\
		ft_lstmap.c

OBJECTS = $(addprefix $(OBJECT_PATH), $(SRC:.c=.o))

INCLUDE = libft.h

.PHONY : all bonus clean fclean re

all: $(NAME)

$(NAME): $(FOBJ_LIBFT) $(OBJECTS)
	@ar rcs $(NAME) $(OBJECTS)

$(OBJECT_PATH)%.o : %.c $(INCLUDE)
	$(CC) $(CFLAGS) -o $@ -c $<

$(FOBJ_LIBFT) : 
	@mkdir $@

clean:
	@rm -f $(OBJECTS)
	@rm -rf $(FOBJ_LIBFT)

fclean: clean
	@rm -f $(NAME)

re: fclean all

