
2025-01-31 03:45

Status: #Finished 

Tags: [[programming language]] [[low-level programming]] [[cybersecurity]]

# Rust Cargo

Rust Cargo is a package manager and a build tool for your code. It does many tasks like building our code, downloading libraries that our code needs, and building those libraries.

We can create a Cargo project using the following command:
```
cargo new *project-name*
```

The new cargo project generated has an src folder with a *main.rs* file and a *Cargo.toml* file. 
==toml==: Tom's Obvious Minimal Language

We refer to packages as **crates** in rust

This is how you run your cargo code:
```
cargo build //this will create another directory called (target). Inside the target folder would be a debug folder inside which your executable file would be
```

```
./target/debug/*project-name*
```

Or you can just run:
```
cargo run
```
Instead of building first and then executing.

**cargo check**: is a command which we can use to see if our code can be compiled but it does not create an executable file

#### References
[[Hello, Cargo! (Rust the book)]]