# PLEASE NOTE:
- **All source code is available for request from hlynch02@tufts.edu**
- To see some of my public source code (albeit not C/C++), see the following repositories:
  - https://github.com/harrylynchh/airtight-container
  - https://github.com/harrylynchh/portfolio
# ------------------------------ C Projects ---------------------------------
# A PGM Reader
1/26/2025

**Summary:**
-------------------------
This project manifested itself in two parts, both relating to the translation of portable gray maps
(pgms) which are a file format outlined in this [spec](https://netpbm.sourceforge.net/doc/pgm.html).
The first part of the project was taking *plain* pgms and turning them into *raw* pgms. The difference
between these two formats is that the former contained human-readable values for raster pixels and the latter
compressed human-readable digits to single bytes (therefore this is for valid raster values from 0-255).
The second half involved taking a "corrupt" plain pgm and translating it back into a valid readable raw pgm.
This mostly involved the parsing of raster digits from corrupt sequences and re-formatting within the netpbm
specification such that images that were previously unintelligible became clear again.
# --------------------------- C++ Projects -------------------------------
# Gerp -- Grep Reimplementation
11/23/2024

**Summary:**
-------------------------

This program is a re-creation of the linux command grep and features a from-scratch
implementation of a template hashtable class.  Given a root directory the program
traverses each subdirectory and all files within.  For each file in the tree, each
word of each line is indexed into a robust, O(n) time access index which can locate
every occurrence of a given word (case sensitive or insensitive) in any file contained
by the root or the root's subdirectories.  This project taught me the ins and outs of
template classes/containers and to be intentional in system design as to prioritize both
time and space efficiency.

# Huffman Encoder/Decoder -- Lossless Compression
11/7/2024

**Summary:**
-------------------------

This program is an implementation of Huffman Coding compression which
takes a tree of weighted characters to encode ASCII chars into a binary string.
This binary string in combination with a serialized version of the Huffman Tree
used to encode the characters is compiled into binary. This binary file can also
be decoded by deserializing the tree from the binary. Then, this tree can be
used as a reference to re-create the original ASCII text.  This project taught
me all about file I/O and how the encoding and decoding process works at its
core.

# Reverse Polish Notation Calculator
10/10/2024

**Summary:**
------------------------------

   This program is an implementation of Reverse Polish Notation (postfix notation)
style calculator which, at its core, uses a basic stack to maintain the order
of operations and execute calculations.  Taking input from cin, the calculator 
is capable of executing boolean comparisons, conditional execution, 
and arithmetic.  Also, note that this calculator is technically turing complete.
This project features a lot of complex stack-based logic that required a modular
and efficient solution to support extensive inputs.

**SEE:** https://en.wikipedia.org/wiki/Reverse_Polish_notation

# Metro Simulator
9/24/24

**Summary**:
---------------
To create a simulation of the Green Line of the Boston T where the user can add
passengers and move the train from station to station with the passengers
boarding and departing at their respective stations.  This project built my
fundamental ability to manage memory with care and security and to keep track
of a rather complex system containing individualized data.
