CC = gcc
CFLAGS = -Wall -Wextra -Iinclude

calculator: main.o calculator.o logger.o
	$(CC) $(CFLAGS) $^ -o $@
	# TODO: link object files into the calculator executable

main.o: src/main.c include/calculator.h include/logger.h
	$(CC) $(CFLAGS) -c $< -o $@
	# TODO: compile src/main.c

calculator.o: src/calculator.c include/calculator.h
	$(CC) $(CFLAGS) -c $< -o $@
	# TODO: compile src/calculator.c

logger.o: src/logger.c include/logger.h
	$(CC) $(CFLAGS) -c $< -o $@
	# TODO: compile src/logger.c

.PHONY: clean
clean:
	rm -f calculator *.o
	# TODO: remove calculator and all .o files
