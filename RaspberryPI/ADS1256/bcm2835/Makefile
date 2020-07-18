all: ads1256_test

ads1256_test: src/*.c src/*.h
	gcc -g -O0 -Wall  src/*.c -lbcm2835 -lm -o ads1256_test

clean :
	rm -f ads1256_test
