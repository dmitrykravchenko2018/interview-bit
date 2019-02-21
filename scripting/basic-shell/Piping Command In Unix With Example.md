Piping Command In Unix With Example
A pipe is a form of redirection that is used in Linux and other Unix-like operating systems to send the output of one program to another program for further processing.

for i in {1..30}; do echo $i; done | cut -c 2 | sort | uniq
Output (generated from for i in {1..30}; do echo $i; done ) which will be taken as input by cut :

1
2
3
.
.
.
28
29
30

The output ( generated by cut -c 2 ) which will be taken as input by sort :

(empty)

.
.
.
8
9
0
The output (generated by sort) which will be taken as input by uniq:



.
.
.
9
9
9
Final output (generated by uniq)


0
1
.
.
.
7
8
9
Note: Run commands separately in the terminal for better understanding.