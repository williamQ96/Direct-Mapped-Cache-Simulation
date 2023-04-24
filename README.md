# Direct-mapped Cache Simulator

This project is a simple C program to simulate a 16B direct-mapped cache with 2B blocks, which results in 8 cache sets. It allows users to read, write, and print the cache.

## Usage

1. Compile the program using a C compiler (e.g., `gcc`):
```sh
gcc -o cache_simulator 8-1.c

2.Run the compiled program:
./cache_simulator

3.Interact with the program by following the prompts:

Enter 'r' to read a value from the cache
Enter 'w' to write a value to the cache
Enter 'p' to print the current state of the cache
Enter 'q' to quit the program

Functions
This program includes the following functions:

getOffset: Extracts the offset bits from a given address
getSet: Extracts the set bits from a given address
getTag: Extracts the tag bits from a given address
mallocCache: Allocates memory for the cache and initializes it
freeCache: Frees the allocated memory for the cache
printSet: Prints the information of a given cache set
printCache: Prints the information of all valid cache sets
readValue: Reads a value from the cache for a given address
writeValue: Writes a new value to the cache for a given address

Example
Enter 'r' for read, 'w' for write, 'p' to print, 'q' to quit: w
Enter 32-bit unsigned hex address: 0x0
Enter 32-bit unsigned hex value: 0xaabb
wrote set: set: 0 - tag: 0 - valid: 1 - data: bb aa
...

License
This project is open source and available under the MIT License.
