Download Link: https://assignmentchef.com/product/solved-csci215-assignment-1-refresher-on-c-programming
<br>
Get a hang of the programming and compilation tools that will be used throughout the semester.

Acquire good habits for assignment submission.

Foreword

This first assignment was deliberately designed to be very easy to solve. If you finish before the end of the session, all the better. If you have trouble answering all the questions in the allotted time, then it is imperative that you brush up your C development skills.

Question 1

Extract the file attached to this assignment, and compile/run the program by calling the make command in the terminal.

Question 2

Edit the Makefile to archive the array implementation of the stack as a library.

The goal is to archive the stack_array.o object file in a library libstack.a

The compilation of the final executable must now be carried out without using the object file stack_array.o

Question 3

We want to change the size of the stack at compile time, via the definition of a constant STACK_SIZE contained in the code.

Use gcc -D directive to change this value from the Makefile, and then get its display in the main program of stack_test.c

Question 4

Using an array is not satisfactory; we would prefer to use a doubly linked list.

Complete the list_impl.c file code to:

<ul>

 <li>Extract an element from the head (the associated cell is removed from the list and the memory it occupied isdeallocated)</li>

 <li>Extract an element from the tail (the associated cell is removed from the list and the memory it occupied is deallocated)</li>

 <li>Compute the number of items in the list</li>

</ul>

<h3>Question 5</h3>

Write a file called stack_list.c that uses the primitives from list.h to build a dynamic stack that implements stack.h

Add a compiler directive in the makefile to build a new library libstack.a from stack_list.c and list_impl.c Recompile an executable from the stack test program (stack_test.c) and use your new library to verify that it works correctly.

<h3>Question 6</h3>

Write a file called fifo_list.c that uses the primitives from list.h to build a dynamic queue that implements fifo.h

Add a compiler directive in the makefile to build a new library libfifo.a from fifo_list.c and list_impl.c

Recompile an executable file from the test program (fifo_test.c) and use your new library to verify that it works correctly.

<h3>Question 7</h3>

Traversing the entire list to determine the number of items is too expensive. What changes should you make, and in which file(s), to determine the size of the list in O(1)?


