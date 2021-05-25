SRC_DIR = src
OBJ_DIR = obj
INC_DIR = inc
EXE_DIR = bin

SRC = $(wildcard $(SRC_DIR)/*.c)
OBJ = $(SRC:$(SRC_DIR)/%.c=$(OBJ_DIR)/%.o)
INC = $(wildcard $(INC_DIR)/*.h)

CC = gcc
exec = exec

all: $(exec)

$(exec): $(OBJ)
	$(CC) -o $(exec) $(OBJ)

$(OBJ_DIR)/%.o: $(SRC_DIR)/%.c
	$(CC) -c $< -I$(INC_DIR) -o $@

.PHONY: clean all

clean:
	@rm exec $(OBJ_DIR)/*.o
