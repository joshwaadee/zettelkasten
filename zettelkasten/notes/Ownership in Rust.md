2023-11-1309:06
Status: #idea
---
Tags: #programming #rust #coding #memory
---

# Ownership in Rust
[[Rust Language Book]]

The system of ownership is how Rust can make memory safety guarantees without needing run-time processes like [[garbage collection]]. It achieves this by applying a set of rules:
- each value in Rust has an *owner*
- there can only be **one** owner at a time
- when the owner goes out of scope, the value will be dropped and the memory is freed

```rust
						// s is not valid here
{
	let s = "hello";    // s is valid from this point on
	
	// do stuff with s
}                       // this scope is over, s isn't valid any more
```

Values can be have temporary ownership by [[Borrowing in Rust]].


---
# References

[Rust Book - Chapter 4](https://doc.rust-lang.org/book/ch04-01-what-is-ownership.html)
