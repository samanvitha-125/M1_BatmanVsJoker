PROJECT_NAME = main

SRC =src\Board.c\
src\TakeTurn.c \
src\Win_game.c \

BUILD = build

#INC=inc
UNI=unity/unity.c

INC	= inc\
-Iunity\

TEST_SRC = test/test_record

PROJECT_OUTPUT = $(BUILD)/$(PROJECT_NAME).out

TEST_OUTPUT = $(BUILD)/Test_$(PROJECT_NAME).out

INCLUDE_LIBS = -lcunit

PROJECT_OUTPUT = $(BUILD)/$(PROJECT_NAME).out

.PHONY: run clean test doc 

$(PROJECT_NAME).exe : $(SRC)
	gcc -I $(INC) $(PROJECT_NAME).c $(SRC)  -o $(PROJECT_NAME).exe

run: $(PROJECT_NAME).exe
	$(PROJECT_NAME).exe

doc:
	make -C ./documentation

clean:
	rm -rf $(BUILD) $(DOCUMENTATION_OUTPUT)

$(BUILD):
	mkdir build