CC = c++ -std=c++98

FLAGS = -Wall -Wextra -Werror -fsanitize=address

MAIN = main.cpp

OBJS = main.o

HEADERS = Array.hpp

NAME = array

all:		$(NAME)

$(NAME):	$(OBJS) $(HEADERS)
			$(CC) $(FLAGS) $(OBJS) -o $(NAME)

$(OBJS): 	$(MAIN) $(HEADERS)
			$(CC) $(FLAGS) $(MAIN) $(HEADERS) -c

clean:		
			rm -rf $(OBJS)
			rm -rf *gch

fclean:		clean
			rm -rf $(NAME)

re:			fclean all

l:			all
			./array