# eecs281-project-1-solved
**TO GET THIS SOLUTION VISIT:** [EECS281 Project 1 Solved](https://www.ankitcodinghub.com/product/eecs281-solved-2/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;122052&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EECS281 Project 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
You have just broken out of the detention level of a large and strangely moon-like space station. You need to find your way back to your old spacecraft of questionable space-worthiness to escape. Your adorable robot friend has hacked into the elevator system of the space station to assist you in your escape.

Learning Objectives

These are the skills and concepts encountered in this project:

3D Maze: read, store, access, and write

Breadth first search (BFS w/ queue)

Depth first search (DFS w/ stack)

Map and coordinate list mode input

Map and coordinate list mode output

Use getopt_long() to handle command line arguments

Command Line Options

ship should take the following (optional) command line options:

–stack , -s

–queue , -q

–output (M|L) , -o (M|L)

Indicates the output file format by the required argument, M (map format) or L (coordinate list format). If this option is not provided when running the program, the default output format is map format. If specified, this option requires that an argument be provided, and the autograder will only use valid arguments.

–help , -h

This causes the program to print a helpful message about how to use the program and then immediately exit(0) .

Legal command lines must include exactly one of –stack or –queue (or their respective short forms -s or -q). If none are specified or more than one is specified, the program should print an informative message to standard error ( cerr ) and exit(1) .

Using getopt_long() will make this much easier. See Project 0 and the man page for getopt, for more information.

Legal Command Lines

$ ./ship –stack &lt; infile &gt; outfile

This will run the program using a stack and map output mode.

$ ./ship –queue –output M &lt; infile &gt; outfile

This will run the program using a queue and map output mode.

$ ./ship –stack –output L &lt; infile &gt; outfile

This will run the program using a stack and coordinate list output mode.

These examples use the shell redirection operators &lt; and &gt; to redirect standard input ( cin ) and standard output ( cout ). This is a convenient way to read input from a file and write output to a file, without having to write any code to open and close files. The operating system “connects”

cin to read the input file, and print statements to cout to the output file.

Illegal Command Lines

$ ./ship –queue -s &lt; infile &gt; outfile

Contradictory choice of routing, both stack and queue are specified.

$ ./ship &lt; infile &gt; outfile

You must specify one of stack or queue options.

$ ./ship -o &lt; infile &gt; outfile

Output option requires an argument describing the output mode.

Space Station Layout

A space station is composed of up to 10 square levels with elevators to travel between levels. The description of a space station will be provided by an input file using a 3-D coordinate system and special characters.

The special characters and what they represent:

ʼ.ʼ floor space ʼ#ʼ walls (the only character that cannot be walked on/through)

‘Sʼ your starting location at the detention level

‘Hʼ the hangar of the spacecraft location (the goal)

‘Eʼ corresponds to elevators that transport you from that location to the same row and column of the levels that have an elevator on the same location

Levels are implicitly enclosed by walls that are not included in input files; you are to treat both level edges and walls as impassable terrain.

Ultimately, your task will be to indicate your route to the hangar tile from your starting location using directional indicators (‘nʼ for north, ‘eʼ for east, ‘sʼ for south, ‘wʼ for west, and 0-9 to indicate where you got off the elevator). More details on this are provided below.

Input File Formats

The program gets its description of the space station from a file that will be read from standard input (cin). This input file is a simple text file specifying the layout of the space station. We require that you make your program compatible with two input modes: Map Mode ( M ) and coordinate list mode ( L ).

The reason for having two input modes is that a large percentage of the runtime of your program will be spent on reading input or writing output. Coordinate list mode exists so that we can express very large graphs with relatively few lines of a file, map input mode exists to express dense graphs (ones for which most of the tiles are not just floor space) in the smallest number of lines. You should use std::ios::sync_with_stdio(false) – this makes a very significant runtime difference.

The first three lines of any input file are called the “file header” and they will be formatted as follows:

The first line of every input file will be a single character specifying the input mode, M or L. Input file format is given in the file, unlike the output mode, which can only be given as a command line option.

The second line will be a single, positive integer 1 ≤ l ≤ 10, indicating the number of levels in the space station.

The third line will be a single, positive integer n ≥ 2, indicating the size of every level of the space station. Each level is n × n in size.

After the file header, the input file will contain the space station layout in one of the two modes listed above and described below.

Map Input Mode

For this input mode, the file header will start with an ‘Mʼ and contain a 2D map of characters defining each level, starting with level 0 and ending with level l − 1.

A map input mode example file for a space station that has two 4×4 levels:

Coordinate List Input Mode

For this input mode, the file header will start with an ‘Lʼ and contain a list of coordinates for at least all non-floor space characters in the space station. A coordinate is specified in precisely the following form: (level,row,column,character). The level values will be in the range [0,l), and the row and column values will be in the range [0,n). Only one coordinate will appear on each line, and there is no guarantee that the coordinates will be grouped by floor or ordered in any way. By default, all unspecified coordinates within the space station are of type ‘.ʼ (floor space); however, it is not invalid to redundantly specify them to be so.

Valid coordinates (for a space station with three 4×4 levels):

Invalid coordinates (for a space station with three 4×4 levels):

A coordinate list input mode example file with two 4×4 levels, equivalent to the example above:

Routing schemes

You are to develop two routing schemes to get from the starting location to the hangar location tile:

A routing scheme that uses a queue as the search container A routing scheme that uses a stack as the search container

Both of these routing schemes will always lead you to the hangar (if a path exists). Whether youʼre supposed to be using stack or queue based, the algorithm is basically the same. Read the “Project 1 the STL and You” file, it will tell you (among many other useful things) how to use a single data structure, a deque, and allow you to write one version of the code for both routing schemes.

Search container (the deque) is where you add things to help you find the hangar. Think of this as the places that might help you get to the hangar, but havenʼt had a chance to investigate yet.

Discovered means that this square has been added to the search container. You can never discover the same location twice (this prevents infinite loops and other problems). You must keep track of what has been discovered and what has not.

Investigate is when a location comes out of the deque, and you start to determine what other locations it helps you to discover. There is no need to track what has or has not been investigated.

Create a search container. Before you start looping, add the starting location to the search container, and mark it as discovered. As long as the search container is not empty, do the following:

. Take the “next location” from the search container; we will refer to this as the current location. Remove it from the search container.

. Investigate the current location. In other words, discover all of the locations that you can reach from the current location. For each one, if it is off the edge, a wall, or already discovered before, ignore it. Otherwise, add it to the search container and mark it as discovered. You should check in this order: N, E, S, W. If the current location is an elevator, you should also discover every other level, from the lowest level (0) to the highest level, in the same row and column as the current location: if any other levels have an ‘Eʼ in the same row/column, and they are not discovered, each should be added to the search container and marked as discovered.

. As soon as you find the hangar tile H, you should stop searching. If you donʼt stop, loop back to step 1.

The only difference between an elevator and a non-elevator tile is what positions you are allowed to discover. You still have to check that you havenʼt discovered a location before discovering it.

One important point to remember: when we talk about the routing scheme, adding things to the search container, etc.: you (the person) are not moving yet! Until your trusty robot companion uses this program to find the route that will get you to the hangar, you stay put. If you start asking questions like “how did I teleport from level 0, row 1, column 2 to level 3, row 5, column 4?”, remember that YOU didnʼt move yet. The program investigated a different location that just happened to be far away from the last location it investigated. Once your robot is done running the program, it will produce output (a map or list of directions) for you to follow, and that set of directions will make sense for you: youʼll go north, go east, take an elevator to level 2, go south, etc.

Output file format

The program will write its output to standard output (cout). Similar to input, we require that you implement two possible output formats. Unlike input, however, the output format will be specified through a command-line option –output, or -o, which will be followed by an argument of M or L (M for map output and L for coordinate list output). See the section on command line arguments below for more details.

For both output formats, you will show the path you took from start to finish.

Map output mode (M):

For this output mode, you should print the map of the levels, replacing existing characters as needed to show the path you took. Beginning at the starting location, overwrite the characters in your path with ‘nʼ, ‘eʼ, ‘sʼ, ‘wʼ, or ‘0-9ʼ (where you got off the elevator) to indicate which tile you moved to next. Elevator tiles that you use in your final path should be overwritten with the number of the level where you exited the elevator. Do not overwrite the ‘Hʼ at the end of the path, but do overwrite the ‘Sʼ at the beginning. For all spaces that are not a part of the path, simply reprint the original space station space. You should discard all existing comments from the input file for the output file. However, do create comments to indicate the level numbers and format them as shown below. Before any other output, state the starting location, so that the map is easier to follow.

Thus, for the sample input file specified earlier, using the queue-based routing scheme and map (M) style output, you should produce the following output:

Using the same input file but with the stack-based routing scheme, you should produce the following output:

Coordinate list output mode (L):

For this output mode, you should print only the coordinates that make up the path you traveled. You should print them in order, from (and including) the starting position to the ‘Hʼ (but you should not print the coordinate for ‘Hʼ). The coordinates should be printed in the same format as they are specified in coordinate list input mode (the (level,row,column,character) format). The character of the coordinate should be ‘nʼ, ‘eʼ, ‘sʼ, ‘wʼ, or ‘0-9ʼ (where you got off the elevator) to indicate spatially which tile is moved to next. You should discard all comments from the input file, but you should add one comment on line 1, just before you list the coordinates of the path that says “//path taken”. Thereʼs no need to state the starting location in this mode, since it would be the first line after the “//path taken”.

The following are examples of correct output format in (L) coordinate list mode that reflect the same solution as the Map output format above:

For the queue solution:

For the stack solution:

There is only one acceptable solution per routing scheme for each map of the space station. If no valid route exists, the program should simply reprint the space station with no route shown for Map output mode, and should have no coordinates listed after the “//path taken” comment in List output mode.

It is extremely frustrating to turn in code that you are ‘certainʼ is functional and then receive half credit. We will be grading for correctness primarily by running your program on a number of test files. If you have a single silly bug that causes most of the test cases on the autograder to fail, you will get a very low score on that part of the project even though you completed 95% of the work.

Most of your grade will come from correctness testing. Therefore, it is imperative that you test your code thoroughly. To help you do this we will require that you write and submit a suite of test files that thoroughly test your project.

Your test files will be used to test a suite of buggy solutions to the project. Part of your grade will be based on how many of the bugs are exposed by your test files. (We say a bug is exposed by a test file if the test file causes the buggy solution to produce different output from a correct solution.)

Each test file should be an input file that describes a space station in either map (M) or coordinate list (L) format. Each test file file should be named test-n-flags.txt where 0 &lt; n &lt;= 15 for each test file. The “flags” portion should include a combination of letters of flags to enable. Valid letters in the flags portion of the filename are:

s: Run stack mode q: Run queue mode m: Produce map mode output l: Produce list mode output

The flags that you specify as part of your test filename should allow us to produce a valid command line. For instance, donʼt include both s and q, but include one of them; include m or l, but if you leave it off, weʼll run in map output mode. For example, a valid test file might be named test-1-sl.txt (stack mode, list output). Given this test file name, we would run your program with a command line similar to the following (we might use long or short options, such as –output instead of -o):

1 ./ship -s –output L &lt; test-1-sl.txt &gt; test-1-output.txt

Errors you must check for

A small portion of your grade will be based on error checking. You must check for the following errors:

Input errors: illegal map characters, such as F. Check this for both map/list input modes.

For coordinate list input mode, you must check that the row, column, and level numbers of each coordinate are all valid.

In all of these cases, print an informative error message to standard error and exit(1). Read the file Error_messages.txt for standard error messages and why to use them. You do not need to check for any other errors.

We will not put extra characters after the end of a line of the map or after a coordinate.

Coordinates in coordinate list input mode will be in the format (level,row,col,character) . There will be exactly one start location ‘Sʼ and exactly one spacecraft hangar tile ‘Hʼ in the space station.

We will not give you the same coordinate twice for the coordinate list input mode.

The input mode line and the integer dimensions of the space station on lines two and three at the beginning of the input file will be by themselves, without interspersed comments, and that they will be correct.

If you see a single ‘/ʼ character at the beginning of a line, you can assume it is a comment. This makes reading the list mode input MUCH easier.

You will never be given negative numbers for the number of levels, the size of the map, or any portion of a coordinate in list input mode. You can assume that all of these numbers will fit within an unsigned int or uint32_t variable.

Submitting your solution

Project Identifier

You MUST include the project identifier at the top of all source and header files that you submit:

// Project Identifier: 950181F63D0A883F183EC0A5CC67B19928FE896A

Do all of your work (with all needed files, as well as test files) in some directory other than your home directory. This will be your “submit directory”. Before you turn in your code, be sure that:

You have deleted all .o files and your executable(s). Typing ‘make cleanʼ shall accomplish this.

The total size of your program and test files does not exceed 2MB.

You donʼt have any unnecessary files or other junk in your submit directory and your submit directory has no subdirectories.

Your code compiles and runs correctly using the g++ compiler. This is available on the CAEN Linux systems (that you can access via login.engin.umich.edu). Even if everything seems to work on another operating system or with different versions of GCC, the course staff will not support anything other than GCC running on CAEN Linux. To keep the compiler used on CAEN in sync with the autograder, we want you to use version 6.2.0 (available on CAEN with the command module load gcc/6.2.0 and/or with a Makefile).

Turn in all of the following files:

All your .h, .hpp, and .cpp files for the project Your test files

You must prepare a compressed tar archive (.tar.gz file) of all of your files to submit to the autograder. One way to do this is to have all of your files for submission (and nothing else) in one directory. Our Makefile provides the command make fullsubmit. Alternately you can go into this directory and run this command:

`tar -czvf ./submit.tar.gz .cpp *.h *.hpp test.txt

This will prepare a suitable file in your working directory.

Note that if youʼre using the Makefile that we provided as part of Project 0 and Lab 1, most of these things will be done for you! When you want to prepare a submission, you can use either ‘make fullsubmitʼ or ‘make partialsubmitʼ. The difference is that a “full submit” includes test files, a “partial submit” does not. Use the command ‘make helpʼ to get our Makefile to tell you everything it can do!

Submit your project files directly to either of the two autograders at: https://g281-

Please make sure that you read all messages shown at the top section of your autograder results! These messages will help explain some of the issues you are having (such as losing points for having a bad Makefile or using disallowed libraries).

When you start submitting test files to the autograder, it will tell you (in the section called “Scoring student test files”) how many bugs exist, the number needed to start earning points, and the number needed for full points. It will also tell you how many are needed to start earning an extra submit/day!

Libraries and Restrictions

Unless otherwise stated, you are allowed and encouraged to use all parts of the C++ STL and the other standard header files for this project. You are not allowed to use other libraries (eg: boost, pthread, etc). You are not allowed to use the regular expressions library (it is not fully implemented on gcc) or the thread/atomics libraries (it spoils runtime measurements). Do not use the STLʼs unique or shared pointers.

Grading

10 points – Test file coverage (effectiveness at exposing buggy solutions).

10 points – Your program does not lose any memory as reported by valgrind. Memory that is “still reachable” is fine, but any of the three types of “lost” will lose points.

Grading will be done by the autograder.

Coding style

Your grade will not be directly based upon your coding style. However, a better coding style will make your code easier to write, debug, and get help on. Good coding style consists of the following:

Clean organization and consistency throughout your overall program

Proper partitioning of code into header and cpp files

Descriptive variable names and proper use of C++ idioms

Effective use of library (STL) code

Omitting global variables, unnecessary literals, or unused libraries

Effective use of comments

Reasonable formatting – e.g an 80 column display

Code reuse/no excessive copy-pasted code blocks

Effective use of comments includes stating preconditions, invariants, and postconditions, explaining non-obvious code, and stating big-Oh complexity where appropriate.

It is extremely helpful to compile your code with the gcc options:

This will help you catch bugs in your code early by having the compiler point out when you write code that is either of poor style or might result in behavior that you did not intend.
