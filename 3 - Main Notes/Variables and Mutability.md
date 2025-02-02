
2025-02-03 01:38

Status: #Finished 

Tags: [[cybersecurity]] [[rust]] [[programming language]] [[low-level programming]]

# Variables and Mutability

- By default, Rust makes your variables immutable. By this we mean that once a value has been assigned to your variable, it cannot be changed.
- Rust encourages you to keep your variables immutable by default because its safe

- Constants and variables are different. You can't use ==mut== with a constant.
- Unlike declaring variables, you use ==const== instead of ==let== 
- Constants naming convention is that their name should be decalred in all caps
- Constants cannot be a return value. It's always set and cannot be changed

- Value of constants are calculated at compile time whereas the values of the variables are calculated at runtime. 

## Shadowing:

Shadowing is when we use the name of the variable for another purpose. For example:

```
let x = 5;
let x = x+1;

println!("The value of x is: {x}");

The output of the above code is: 6
```

In the above code we "Shadowed" the initial x variable by changing its value from x = 5 to x = 6.
- Shadow variables carry on the final value until the end of the scope or if they're further shadowed by another variable.



#### References
[[Variables and Mutability (Rust the book)]]