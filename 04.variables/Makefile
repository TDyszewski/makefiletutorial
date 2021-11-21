files = file1 file2
x = dude

some_file: $(files)
	echo "Look at this variable: " $(files)
	touch some_file

file1:
	touch file1
file2:
	touch file2

clean:
	rm -f file1 file2 some_file

all:
	echo $(x)
	echo ${x}

	# Bad practice but works
	echo $x

