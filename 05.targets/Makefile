all: one two three

all_f: f1.o f2.o

one:
	touch one

two:
	touch two

three:
	touch three

clean:
	rm -f one two three hey

f1.o f2.o:
	echo $@

print: $(wildcard *.c)
	ls -la

hey: one two
    # Outputs "hey", since this is the first target
#    echo $@

	# Outputs all prerequisites newer than the target
	echo $?

	# Outputs all prerequisites
	echo $^

	touch hey
