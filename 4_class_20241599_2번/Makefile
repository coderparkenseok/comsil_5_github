cc = gcc
target = animal_exe
objects = dog.o blackcow.o turtle.o main.o

$(target): $(objects)
	$(cc) -o $(target) $(objects)

dog.o: dog.c animal.h
	$(cc) -c -o dog.o dog.c

blackcow.o: blackcow.c animal.h
	$(cc) -c -o blackcow.o blackcow.c

turtle.o: turtle.c animal.h
	$(cc) -c -o turtle.o turtle.c

main.o : main.c animal.h
	$(cc) -c -o main.o main.c

.PHONY : clean
clean:
	rm -f $(target) $(objects)
