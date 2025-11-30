---
layout: page
title: Final exam guide
nav_order: 5
description: >-
    Final exam guide.
---

# CIS241 - F2025 Final Exam Study Guide

## All material from the midterm onward (i.e., starting with regex) is valid for questions

* In-class discussions/demos
* Homeworks
* In-class assignments
* Slides

## Things to know

* You can bring a 1-page cheat sheet, front and back.  You'll need to turn it in with your exam, so if you want it back put your name on it.

* The exam is hand-written - no devices allowed.

* The exam will comprise a number of theory (what you understand) and practical (do a thing) types of questions.
  * For the practical questions, I'll provide a reference guide on the back of the exam.

## Sample topics

**Note - this is not comprehensive - anything is valid from the slides/assignments**

* What is the purpose of regex?  How could you use it in a script?
* What is the purpose of using tmux/screen? Give an example of its use.
* What is the purpose of compiling a C program?  How is a compiled file different from programs in languages like Java or Python?
* If I build a binary file with `gcc`, can I simply give it to you to run?  What would I have to do to make sure it works for you?
* What is the purpose of a `#include` block?  What happens if I try to call `printf` without `#include <stdio.h>`?
* What is a preprocessor directive?
* Are the semi-colons *actually* required?
* How do you run a program?
* How do you compile a program?  Compile with extra warnings displayed?  Compile to a named binary file?
* Why do we worry about how many bits a variable has?  How large of a number does a 32-bit unsigned integer allow?  What if it were signed?
* Boolean doesn't exist *by default* - describe two ways you could use a Boolean in C.
* What is a pointer?  Why bother using one?  Give an example.
* How can you be sure that dynamically-allocated memory is initialized to 0?  To another value?
* What are `int argc, char* argv[]`?
* How do you convert a `char` to an `int`?
* What is the difference between `&` and `*` with respect to pointers?
* What is variable scope?
* Describe what the stack and what the heap are.
  * If I use statically-defined variables (e.g., `int x`), where is that memory stored?
  * If I use `malloc`, where is that memory stored?
* Be able to follow a C program and describe what is happening (could be looping, could be pointer math, etc.).
* What is the difference between a function prototype and function definiton? 
* What is pass-by-reference and pass-by-value?  What does C natively do (i.e., without pointers)?
* What is the purpose of using `free` to clear up memory created with `malloc`/`calloc`?
* What are some memory-specific concerns one would have with reading user input?  
* What is the purpose of a `struct`?  What is the purpose of a `union`?
* Why would we use `typedef`?
* What is the purpose of debugging?  Why would we use `gdb` over trace debugging (i.e., print statements)?
* What are *header guards*?  Why do we need them?
* Are 2D arrays always contiguous in memory?  Is it a problem if they aren't?  How would you access data if they weren't (i.e., if you couldn't do `arr[1][4]`)?
* What is the purpose of a makefile?  Describe three actions you can do with it.
* Describe two uses of the string library.
* Describe how you would read and write from/to a file.
* What is the purpose of an `enum`?

## Sample practical questions

**Note - this is not comprehensive - anything is valid from the slides/assignments**

* Define a regex that matches an input (using extended regular expressions as we did in class)

* In C, be able to:
  * Read and use command-line arguments
  * Print output to the terminal (ints, strings, chars, etc.)
  * Use preprocessor directives to define variables, check if they exist, etc.
  * Create, initialize, and use a 1D array
  * Create, initialize, and use a 2D array
  * Create *dynamic* memory of a specified size and type.
  * Create and use a header file **with** header guards
  * Handle user input (characters, integers, or strings)
  * Create and use a struct
  * Define and call functions
  * Read and write a file
  * Use control/loop statements (`if`, `for`, `while`, etc.).
  * Create a variable, create a pointer to that variable, and update the original variable's value via the pointer.
  * Access an array via index and via a pointer
  * Pass a struct to a function and update it
  * Define a makefile that builds a target binary, builds an intermediate binary, and cleans up its mess.