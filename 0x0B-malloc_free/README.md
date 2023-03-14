C - MALLOC, FREE
This README provides information about the C programming language's dynamic memory allocation functions malloc() and free().
Memory allocation is a crucial aspect of programming, especially when it comes to managing large data structures, such as arrays or linked lists. The dynamic memory allocation functions in C allow you to allocate and free memory during program execution dynamically.

Malloc():
The malloc() function in C is used to dynamically allocate a block of memory in the heap.
It takes one argument, the number of bytes to be allocated, and returns a void pointer (void*) to the first byte of the allocated block if successful.
Otherwise, it returns NULL if there is not enough memory available to satisfy the request.
Free():
The free() function is used to deallocate a block of memory previously allocated by malloc().
It takes a pointer to the block of memory to be freed as its argument.
COMCLUTION
Dynamic memory allocation is an essential feature of the C programming language, allowing for the creation of data structures whose size can be determined at runtime. The malloc() and free() functions allow for the allocation and deallocation of blocks of memory during program execution, making it possible to manage memory efficientl

MALLOC AND FREE
TASK 0
Float like a butterfly, sting like a bee
Write a function that creates an array of chars, and initializes it with a specific char.

Prototype: char *create_array(unsigned int size, char c);

Returns NULL if size = 0

Returns a pointer to the array, or NULL if it fails.

TASK 1
The woman who has no imagination has no wings
Write a function that returns a pointer to a newly allocated space in memory, which contains a copy of the string given as a parameter.

Prototype: char *_strdup(char *str);

The _strdup() function returns a pointer to a new string which is a duplicate of the string str. Memory for the new string is obtained with malloc, and can be freed with free.

Returns NULL if str = NULL

On success, the _strdup function returns a pointer to the duplicated string. It returns NULL if insufficient memory was available

TASK 2
He who is not courageous enough to take risks will accomplish nothing in life
Write a function that concatenates two strings.

Prototype: char *str_concat(char *s1, char *s2);

The returned pointer should point to a newly allocated space in memory which contains the contents of s1, followed by the contents of s2, and null terminated

if NULL is passed, treat it as an empty string

The function should return NULL on failure

TASK 3
If you even dream of beating me you'd better wake up and apologize
Write a function that returns a pointer to a 2 dimensional array of integers.

Prototype: int **alloc_grid(int width, int height);

Each element of the grid should be initialized to 0

The function should return NULL on failure

If width or height is 0 or negative, return NULL

TASK 4
It's not bragging if you can back it up
Write a function that frees a 2 dimensional grid previously created by your alloc_grid function.

Prototype: void free_grid(int **grid, int height);
Note that we will compile with your alloc_grid.c file. Make sure it compiles.
ADVANCED
TASK 5
It isn't the mountains ahead to climb that wear you out; it's the pebble in your shoe
Write a function that concatenates all the arguments of your program.

Prototype: char *argstostr(int ac, char **av);

Returns NULL if ac == 0 or av == NULL

Returns a pointer to a new string, or NULL if it fails

Each argument should be followed by a \n in the new string

TASK 6
I will show you how great I am
Write a function that splits a string into words.

Prototype: char **strtow(char *str);

The function returns a pointer to an array of strings (words)

Each element of this array should contain a single word, null-terminated

The last element of the returned array should be NULL

Words are separated by spaces

Returns NULL if str == NULL or str == ""

If your function fails, it should return NULL
