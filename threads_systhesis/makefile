GG = g++
CPPFLAGES = -std=c++0x -pthread

CPPRCS := $(wildcard *.cpp)
OBJS := $(CPPRCS:%.cpp=%.o)

main: main.o module.o
	$(GG) $(CPPFLAGES) -o $@ $^
	@echo $@

%.o: %.cpp
	$(GG) $(CPPFLAGES) -c $< -o $@
	@echo $@

.PHONY: clean
clean:
	rm -rf *.o main
