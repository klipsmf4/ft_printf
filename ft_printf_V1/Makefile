# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: kbarahon <kbarahon@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2020/10/11 19:47:39 by kbarahon          #+#    #+#              #
#    Updated: 2020/10/19 20:55:31 by kbarahon         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libftprintf.a

SRCS = ft_atoi.c ft_inspector_format.c ft_isalpha.c ft_isdigit.c \
		ft_num_len.c ft_printf.c ft_strcmp.c get_data_type.c init_values_t_var.c \
		print_caracter.c print_percentage.c print_zero_space.c put_fuctions.c \
		reset_values_t_var.c spect_format.c get_flags.c str_functions.c get_precision.c \
		get_width.c print_string.c print_decimal.c print_unsigned.c print_hexadecimal.c \
		int_to_hex.c print_pointer.c int_to_hex_long_un.c

OBJS        =   ${SRCS:.c=.o}

CC          =   gcc

CFLAGS      =   -c -Wall -Wextra -Werror -g

RM			=	rm -f

all:		$(NAME)

$(NAME):	${SRCS}
	${CC} ${CFLAGS} ${SRCS}
	ar -rc ${NAME} ${OBJS}
	ranlib ${NAME}

clean:	
	${RM} ${OBJS}

fclean:		clean
	${RM} ${NAME}

re:			fclean all

.PHONY:		all clean fclean re