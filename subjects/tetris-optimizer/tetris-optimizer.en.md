## tetrisoptimizer

### Objectives

Develop a program that receives only one argument, a path to a text file which will contain a list of [tetrominoes](https://en.wikipedia.org/wiki/Tetromino) to assemble them in order to create the smallest square possible.

### Instructions

The program must :

-   Be written in Go
-   Compile successfully
-   Assemble all of the tetrominoes in order to create the smallest square possible
-   Identify each tetromino in the solution by printing them with uppercase latin letters (`A` for the first one, `B` for the second, etc)
-   Expect at least one tetromino in the text file
-   In case of bad format on the tetrominoes or bad file format it should print `ERROR`

#### Example of a text File

```console
#...
#...
#...
#...

....
....
..##
..##
```

-   If it isn't possible to form a complete square, the program should leave spaces between the tetrominoes. For example:

```console
ABB.
ABB.
A...
A...
```

## Usage

```
student@ubuntu:~/tetrisoptimizer$ cat -e sample.txt
...#$
...#$
...#$
...#$
$
....$
....$
....$
####$
$
.###$
...#$
....$
....$
$
....$
..##$
.##.$
....$
$
....$
.##.$
.##.$
....$
$
....$
....$
##..$
.##.$
$
##..$
.#..$
.#..$
....$
$
....$
###.$
.#..$
....$
student@ubuntu:~/tetrisoptimizer$ ./tetrisoptimizer sample.txt | cat -e
ABBBB.$
ACCCEE$
AFFCEE$
A.FFGG$
HHHDDG$
.HDD.G$
student@ubuntu:~/tetrisoptimizer$
```
