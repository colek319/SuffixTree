CXX = clang++

CXXFLAGS = -Wall -Wextra -std=c++17 

all: test

test: SuffixNode.o SuffixEdge.o SuffixTree.o test.o 
	$(CXX) $(CXXFLAGS) -o test SuffixNode.o SuffixEdge.o SuffixTree.o test.o 

test.o: ../src/test.cpp ../include/SuffixNode.h ../include/SuffixEdge.h ../include/SuffixTree.h
	$(CXX) $(CXXFLAGS) -c ../src/test.cpp

SuffixNode.o: ../src/SuffixNode.cpp ../include/SuffixNode.h
	$(CXX) $(CXXFLAGS) -c ../src/SuffixNode.cpp

SuffixEdge.o: ../src/SuffixEdge.cpp ../include/SuffixEdge.h
	$(CXX) $(CXXFLAGS) -c ../src/SuffixEdge.cpp 

SuffixTree.o: ../src/SuffixTree.cpp ../include/SuffixTree.h
	$(CXX) $(CXXFLAGS) -c ../src/SuffixTree.cpp

clean:
	rm -rf test *.o



