CC = c++

RM = rm -f

CFLAGS = -Wall -Wextra -Werror -std=c++98 

NAME = convert 

SRCDIR = ./srcs

SRC = $(wildcard *.cpp)

OBJ = $(SRC:.cpp=.o)

all:
	@$(MAKE) -j $(NAME)	

$(NAME): $(SRC)
	$(CC) $(CFLAGS) $(SRC) -o $(NAME)

%.o : %.cpp
	$(CC) -c $(CFLAGS) $(SRC) $< -o $@ 

clean:
	$(RM) $(OBJ)

fclean: clean
	$(RM) $(NAME)

re: fclean all

.PHONY: all clean fclean re
