# Functions

* Rust uses snake case (i.e., this_is_snake_case)

* You can declare a function with parameters as so:
  ```
    fn main() {
      another_function(5);
    }

    fn another_function(x: f32) {
      println!("The value of x is: {x}");
    }
  ```
  1. The 'x' variable in another_function() is called a parameter
  2. The concrete value of 5 that is passed when another_functon() is called upon is referred to as an argument

## Statements and expressions

* Rust is a statement-based language

* Statements
  1. Instructions that perform some action and do not return a value
  2. They end with a semi-colon
  3. Examples:
     1. ```let y = 6;```
     2. ``` println!("Hello world!");```

* Expressions
  1. Evaluate to a resultant value 
  2. They do not end with a semi-colon
  3. Examples:
     1. ```5+6```
     2. ```5```

## Comments

* In Rust you comment via the use of double forward slashes: ```// this is a comment```