CXXFLAGS = -Wall -Wextra -g -O2 -std=c++11

FBO: main.o tga.o gl-utils.o matrix.o
	g++ $^ -o $@ -lglut -lGLEW -lGL -pthread

clean:
	@rm -f *o *~ FBO

gl-utils.o: gl-utils.cc gl-utils.h
main.o: main.cc gl-utils.h matrix.h image.h
matrix.o: matrix.cc matrix.h
tga.o: tga.cc image.h
