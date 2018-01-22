[Rust Programming language](https://doc.rust-lang.org/book/second-edition/ch01-00-introduction.html)<br>

Memory corruption:<br>

C and C++ have powerful features of explicit memory management and pointer arithmetic => mem corruption<br> 


1. Using uninitialized memory: Contents of uninitialized memory are treated as garbage values. Using such values can lead to unpredictable program behavior.

2.Using none-owned memory: It is common to use pointers to access and modify memory. If such a pointer is a null pointer, dangling pointer (pointing to memory that has already been freed), or to a memory location outside of current stack or heap bounds, it is referring to memory that is not then possessed by the program.

3.Using memory beyond the memory that was allocated (buffer overflow): If an array is used in a loop, with incorrect terminating condition, memory beyond the array bounds may be accidentally manipulated.

4. Faulty heap memory management: Memory leaks and freeing non-heap or un-allocated memory are the most frequent errors caused by faulty heap memory management.

Memory leaks:  memory which is no longer needed is not released<br>
A memory leak reduces the performance of the computer by reducing the amount of available memory.<br>

**RAII**, short for Resource Acquisition Is Initialization, is an approach to the problem unlike garbage collection<br>
But still memory is finite and will lead to slowing system happen. => **segmentation fault(memory full)**

