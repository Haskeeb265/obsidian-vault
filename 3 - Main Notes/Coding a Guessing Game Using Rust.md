
2025-02-01 14:31

Status: #InProgress 

Tags:[[low-level programming]] [[cybersecurity]] [[rust]]

# Coding a Guessing Game Using Rust

- We start by importing the **io** library from the **std** (standard) library. This helps us in taking input from the user. We start every code by importing such libraries. 
- There are some items like the **io** library which Rust includes in every code. That set of items is called a *prelude*
- If an item that you want to use isn't included in the *prelude*, you'll have to explicitly call it using the ==use== statement
 - By default, all variables in Rust are immutable. This means that their assigned values never change. To make these variables dynamic, we use the ==mut== keyword after the ==let== keyword when creating a variable
   
 - **Associated Functions**: Associated functions are referred to by ==::==. For example: 
```
 let mut guess = String::new();
```
In the above code, ==new== is an associated function of ==String==

- In short, in the above code, we created a new mutable variable using ==let== which we named guess. Then we declared that the guess variable is currently an 

**Cargo.lock** helps us with producing reproduceable codes. What we mean by that is when you build your code, Cargo figures out the dependencies that fit the criteria of your code and save them in the Cargo.lock file. What this does is even if a new version of that dependency was to come out tomorrow, Cargo would use the specified version of that dependency from your Cargo.toml. This allows Rust to not recompile the code from scratch every time and rather only focus on the new changes. 


- *Shadowing:* Shadowing is a property in Rust which allows us to use the names of previous variables.
#### References
[[Programming a Guessing Game (Rust the book)]]