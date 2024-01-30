# Data Types
* Rust is a compile language; so it must know the data types of all variables at compile time.

## Scaler
* They represent a single value
* Integers
	* signed: i8, i16, i32, etc...
* Floating-point numbers
	* unsigned: u8, u16, u32, etc...
* Booleans
	* True or False
* Characters
	* 'z', 'etc', (note that they are expressed with single quotes)

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

# Comments

* In Rust you comment via the use of double forward slashes: ```// this is a comment```




# Control FLow templates

##  if Expressions

```
fn main() { 
	let number = 3; 
	if number < 5 { 
		println!("condition was true"); 
	} else { 
		println!("condition was false"); 
	} 
}
```

```
fn main() {
	let number = 6;
	if number % 4 == 0 {
		println!("number is divisible by 4");
	} else if number % 3 == 0 {
		println!("number is divisible by 3");
	} else if number % 2 == 0 {
		println!("number is divisible by 2:);
	} else {
		println!("number is not divisible by 4, 3, or 2");
	}
}
```



## loops

```
fn main() {
	let mut counter = 0;

	let result = loop {
		counter += 1;

		if counter == 10 {
			break counter * 2;
		}
	};

	println!("The result is {result}");
}
```



## while loops

```
fn main() {
	let mut number = 3;
	
	while number != 0 {
		println!("{number}!");

		number -= 1;
	}

	println!("LIFTOFF!!!");
}
```



## for loops

```
fn main() {
	for number in (1..4).rev() {
		println!("{number}!");
	}
	println!("LIFTOFF!!!");
}
```
