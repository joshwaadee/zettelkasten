2023-11-1311:22
Status: #inbox
---
Tags: #programming #coding #rust #memory 
---

# Borrowing in Rust
[[Rust Language Book]]

If we need to use a value without taking ownership, we can borrow that value by referencing it. A Variable in can have three kinds of permission: Read, Write and Ownership. By default, a value has the Read and Ownership permissions and in order for a variable to have Write permissions we have to declare it as mutable with `let mut`. **A variable can be aliased with a reference. A variable can be mutated. Variables cannot be *both* aliased *and* mutated.**

- At any given time you can have *either* one mutable reference or any number if immutable references

---
# References

[Rust Book - Chapter 4](https://doc.rust-lang.org/book/ch04-02-references-and-borrowing.html)