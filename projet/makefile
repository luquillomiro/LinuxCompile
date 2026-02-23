all: codeComp

codeComp: Comp/testLib.o Comp/new.o
	g++ -o codeComp Comp/new.o Comp/testLib.o

Comp/testLib.o: src/testLib.cpp
	g++ -c src/testLib.cpp -o Comp/testLib.o 

Comp/new.o: src/new.cpp lib/testLib.h
	g++ -c src/new.cpp -o Comp/new.o

clean:
	rm -rf Comp/*.o

mrproper: clean
	rm -rf codeComp
