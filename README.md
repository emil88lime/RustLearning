# RUST Online Tutorial
### Initial README for testing

This is an attempt to create a basic tutorial on Rust Programming Language with the aim to reach a level of understanding by implementing smaller development tools and reusable code.

### Rust Initialization

The first command to run is the following:

> cargo init

This will result to the creation of the following structure:

your-project/

├── README.md

├── .gitignore

├── Cargo.toml

└── src/

└── main.rs

1. main.rs sees mod features;
2. Rust loads the features module
3. Then inside features, the mod.rs file says pub mod print;, which tells Rust to include print.rs and make it accessible from outside features
4. main.rs can call features::print::show_message();

IMPORTANT NOTE: All the commands in Rust must end with `;`

## Print Macro

Rust uses the `println!` macro to print the text to the console.

Example:  
_Print string_  
`println!("Hello World!");`  
_Print string and variable_  
`println!("Number {x}");`

## Variables  

Variables are _immutable_ by default in Rust. A value needs to be bound to a name and then it cannot be changed.  
If you want them to become _mutable_ you need to add `mut` in the front of the variable name. 

### Defining variables

Examples:
_Immutable_  
`let x : i32 = 10;`  
_Mutable_  
`let mut y : i32 = 9`  
If we try to assign a new value to the variables `x` and `y` like this:  
`x = 11` //This will fail the compilation
`y = 5` //This will work

