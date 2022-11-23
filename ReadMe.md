# Common Concepts On Rust Programming 

# Mutability 

When you declare a variable you must specify if this variable is mutable or immutable. The following code will crash beacause of the absecence of the **mut** property 

*let x = 5;*
    *println!("The value of x is: {}", x);*
    *x = 6;*
    *println!("The value of x is: {}", x);*

**To make it work you just need to declare the mut property like this**
*let **mut** x = 5*

## Constants 

Constant variables are declared with the **const** property instead of **let**. Constants can also be declared outside of a function.
Rust’s naming convention for constants is to use all uppercase with underscores between words.
## SHADOWING

You can shadow a variable by declaring it again with **let** property. You can also shadow multiple times for multiple uses, but considering the shadows as the layers of an onion you start from the core of the onion. **You will be shadowing from the last shadow you declared**

# Data Types

Every value in Rust is of a certain data type, which tells Rust what kind of data is being specified so it knows how to work with that data, that means is a statically typed language 

We have Scalar, and compuound types