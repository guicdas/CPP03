CXX				= c++
CXXFLAGS			= -Wall -Wextra -Werror -std=c++98
RM				= rm -fr
INC				= -I includes/*.hpp
NAME			= RepetitiveWork

SOURCES			= main.cpp ClapTrap.cpp ScavTrap.cpp FragTrap.cpp

SOURCES_O		= $(SOURCES:.cpp=.o)

all:			$(NAME)

$(NAME):	$(SOURCES)
	@$(CC) $(CFLAGS) $(INC) $(SOURCES) -o $(NAME)
clean:
	@$(RM) $(SOURCES_O)

fclean:			clean
	@$(RM) $(NAME)

re:				fclean $(NAME)

exe:
	clear
	@$(RM) $(SOURCES_O)
	@$(RM) $(NAME)
	@$(CC) $(CFLAGS) $(INC) $(SOURCES) -o $(NAME)
	@./$(NAME)

.PHONY:			all clean fclean re exe