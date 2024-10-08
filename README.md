# Read Characters from File

Learning Goals 
==============

This assignment asks you to write a program that reads characters from a file.

You will learn to
* Read characters from file
* Understand file permission
* Convert between number of character by the ASCII table
* Handle errors (when fopen fails)

Read Data from File
===================

Files provide permanent storage of information. Before reading from or
writing to a file, a file has to be opened (by calling `fopen`). When
a file is no longer used, it need to be closed (by calling `fclose`).

Calling `fopen` may fail for several reasons. If `fopen` wants to read
a file, the file may not exist. It is also possible that the file
exists but cannot be read due to permission settings. If `fopen` wants
to write a file, the file may exist but it is read-only. It is also
possible that there is no space available on the disk.

What you need to do
===================

You need to write a function called `countChar(char * filename, int *
counts, int size)` that opens a file named `filename`. If `fopen` fails
return false, *DO NOT* `fclose`.

You have to store the count of each
character in the count array. Further instructions are in the comments
in the function in file `filechar.c`

You also need to write a function called `printCounts(int * counts,
int size)` that prints out the count of each character.  Further
instructions are in the comments in the function in file `filechar.c`

Test Your Program
=================

You must test whether your program can handle unexpected situations, such as

* No name of the input file (argc < 2)
* The input file cannot be open
* You must not assume that `size` is 256

Your program must not crash for these situations.

PS: The program output name can be anything. That does not affect the program. 

Submission Instructions
=======================
Zip up only filechar.c for each part using the zip command and submit on gradescope.
