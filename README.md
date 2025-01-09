# Unsafe Raw Pointer and Vector Reallocation in Rust

This repository demonstrates a common error in Rust involving the unsafe use of raw pointers with vectors.  Modifying a vector's contents through a raw pointer after the vector has been reallocated or dropped leads to undefined behavior.  The example code shows how this can happen and provides a safer solution.

The `bug.rs` file contains the buggy code that showcases this issue.  The `bugSolution.rs` file demonstrates a corrected version of the code that avoids the use of raw pointers and instead utilizes safer Rust mechanisms for accessing and modifying vector elements.