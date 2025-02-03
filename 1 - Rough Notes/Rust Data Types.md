
2025-02-04 03:17

Status: #InProgress  

Tags: [[cybersecurity]] [[rust]] [[programming language]] [[low-level programming]]

# Rust Data Types

Rust datatypes are divided into two subsets:
1. Scalar
2. Compound

- Rust is a statically typed language. This means that Rust should know all the data types on compile time. 
- Like python, Rust can also infer what type we want to use based on the value of the variable. However it is suggested to explicitly declare the datatypes of your variables.

### Scaler Types:

Scalar types represents a single value. Rust has 4 primary scalar types:
1. Integers
2. Floating-point numbers
3. Booleans
4. Characters

- There are 2 types of integers in Rust. Signed and Unsigned.
- Signed variables means that the variable can be a negative integer. (- sign). Signed integer is denoted by ==i==. i8, i16, i32, i64 and so on are signed integers
- If the integer is to stay positive, we'll make it an unsigned integer. Unsigned integers are denoted by  ==u==. u8, u16, u32, u64 and so on are unsinged integers.

- Each signed variant can store this many numbers:
**-(2^n-1) to 2n^-1** where **n** = bit architecture (8,16,32,64...)
- Each unsinged variant can store this many numbers:
**0 to 2n^-1**


- Floating-point numbers only have 2 types: ==f32== and ==f64==
#### References
[[Data Types (Rust the book)]]