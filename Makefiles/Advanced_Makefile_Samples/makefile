# Macros
DEPS1 = g++ -std=c++11 -I headers/ cpps/class.cpp
DEPS2 = g++ -std=c++11 -I headers/ class.o

# Compile and assemble files.
# Compiles and links files and generates executable target file named COSC4348.
# Remove all the object files created while compiling.

COSC4348: cpps/class.cpp cpp1/main.cpp 
	$(DEPS1) cpp1/main.cpp -c 
	$(DEPS2) main.o -o exec/COSC4348
	rm class.o main.o 

COSC4354: cpps/class.cpp cpp2/main.cpp
	$(DEPS1) cpp2/main.cpp -c
	$(DEPS2) main.o -o exec/COSC4354
	rm class.o main.o

COSC3346: cpps/class.cpp cpp3/main.cpp
	$(DEPS1) cpp3/main.cpp -c
	$(DEPS2) main.o -o exec/COSC3346
	rm class.o main.o

# Execute the program COSC4348 located in the exec directory.
RunCOSC4348: exec/COSC4348
	./exec/COSC4348

RunCOSC4354: exec/COSC4354
	./exec/COSC4354

RunCOSC3346: exec/COSC3346
	./exec/COSC3346

# Remove the executable file names COSC4348 located in the exec directory.
CleanCOSC4348: 
	rm exec/COSC4348

CleanCOSC4354:
	rm exec/COSC4354

CleanCOSC3346:
	rm exec/COSC3346

# Remove all the executable files that could be created in this makefile.
Cleanall:
	rm exec/COSC4348 exec/COSC4354 exec/COSC3346

