all: myexp

logger.o: logger.cpp logger.h CS149intrin.h CS149intrin.cpp
	g++ -c -g -Ddebug logger.cpp

CS149intrin.o: CS149intrin.cpp CS149intrin.h logger.cpp logger.h
	g++ -c -g -Ddebug CS149intrin.cpp

myexp: CS149intrin.o logger.o main.cpp
	g++ -g -Ddebug -I../common logger.o CS149intrin.o main.cpp -o myexp

clean:
	rm -f *.o myexp *~
