NAME        =	libft.a

SRCS		=	ft_memset.c				\
				ft_bzero.c				\
				ft_memcpy.c				\
				ft_memccpy.c			\
				ft_memmove.c			\
				ft_memchr.c				\
				ft_memcmp.c				\
				ft_strlen.c				\
				ft_isalpha.c			\
				ft_isdigit.c			\
				ft_isalnum.c 			\
				ft_isascii.c			\
				ft_isprint.c			\
				ft_toupper.c			\
				ft_tolower.c			\
				ft_strchr.c				\
				ft_strrchr.c			\
				ft_strncmp.c			\
				ft_strlcpy.c			\
				ft_strlcat.c			\
				ft_strnstr.c			\
				ft_atoi.c				\
				ft_calloc.c				\
				ft_strdup.c				\
				ft_substr.c				\
				ft_strjoin.c			\
				ft_strtrim.c			\
				ft_split.c				\
				ft_itoa.c				\
				ft_strmapi.c			\
				ft_putchar_fd.c			\
				ft_putstr_fd.c			\
				ft_putendl_fd.c			\
				ft_putnbr_fd.c			\
				ft_putchar.c			\
				ft_putstr.c				\
				ft_strndup.c

OBJS		=	$(SRCS:.c=.o)

SRCSBONUS	=	ft_lstnew.c			\
				ft_lstadd_front.c	\
				ft_lstsize.c		\
				ft_lstlast.c		\
				ft_lstadd_back.c	\
				ft_lstdelone.c		\
				ft_lstclear.c		\
				ft_lstiter.c		\
				ft_lstmap.c

OBJSBONUS	=	$(SRCSBONUS:.c=.o)

CC			=	@clang

CFLAGS      =	-Wall -Wextra -Werror

RM			=	@rm -f

.c.o:
			$(CC) $(CFLAGS) -c $< -o $(<:.c=.o)

all:		$(NAME)

$(NAME):	$(OBJS)
			@ar rc $(NAME) $(OBJS)
			@echo "\033[1;30m[$(NAME)] \033[1;32mcreated !\033[0m"

bonus:		$(OBJS) $(OBJSBONUS)
			@ar rc $(NAME) $(OBJS) $(OBJSBONUS)

clean:
			$(RM) $(OBJS) $(OBJSBONUS)

fclean:		clean
			$(RM) $(NAME)

re:			fclean all

.PHONY:		bonus all clean fclean re
