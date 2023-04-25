# Dynamic memory allocation is a feature in the C programming language that allows you to allocate memory for variables at runtime, rather than at compile-time. It enables you to allocate and deallocate memory dynamically during the execution of a program, which can be useful for scenarios where the memory requirements are not known at compile-time or need to change dynamically during program execution.

In C, dynamic memory allocation is done using four key functions:

malloc(): This function is used to dynamically allocate memory from the heap (a region of memory used for storing data that is not tied to a specific scope or lifetime). It takes the size of the memory block to be allocated as an argument and returns a pointer to the first byte of the allocated memory block. If the allocation fails, malloc() returns a NULL pointer.

calloc(): This function is similar to malloc(), but it also initializes the allocated memory block to zero. It takes two arguments - the number of elements to be allocated and the size of each element - and returns a pointer to the first byte of the allocated memory block. If the allocation fails, calloc() returns a NULL pointer.

realloc(): This function is used to resize a previously allocated memory block. It takes a pointer to the previously allocated memory block, the new size of the memory block, and returns a pointer to the first byte of the resized memory block. The contents of the old memory block are preserved in the new block up to the minimum of the old and new sizes. If the allocation fails, realloc() returns a NULL pointer.

free(): This function is used to deallocate memory that was previously allocated using malloc(), calloc(), or realloc(). It takes a pointer to the memory block to be deallocated as an argument and releases the memory back to the heap, making it available for other parts of the program to use.
