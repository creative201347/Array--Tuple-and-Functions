## Tuples
A tuple is a collection of values of different types. Tuples are constructed using parentheses `()`, and each tuple itself is a value with type signature `(T1, T2, ...)`, where T1, T2 are the types of its members. Functions can use tuples to return multiple values, as tuples can hold any number of values.
```rs
fn main() {
    let a = (100, 12, "Nabin", false);
    let mixture = ("Hello, World!", 16, 2.71828);

    println!("{:?}", a);
    println!("{:?}", a.0);
    
    // destructuring a tuple
    let (message, number, float) = mixture;
}
```

## Array
An array is a collection of objects of the same type `T`, stored in contiguous memory. Arrays are created using brackets `[]`, and their length, which is known at compile time, is part of their type signature `[T; length]`.
```rs
fn main() {
    let a = [1, 2, 3];
    let b = ["Nabin", "Dhami"];
    let arr = [1, 2, 3];

    for i in arr.iter() {
        println!("{:?}", i)
    }

    for i in 0..3 {
        println!("{:?}", arr[i])
    }
}
```


## Functions
Functions are prevalent in Rust code. You’ve already seen one of the most important functions in the language: the `main` function, which is the entry point of many programs. You’ve also seen the `fn` keyword, which allows you to declare new functions.
Rust code uses `snake case` as the conventional style for function and variable names, in which all letters are lowercase and underscores separate words. 
```rs
fn main() {
    let x = plus_one(5);
    println!("The value of x is: {x}");
}

fn plus_one(x: i32) -> i32 {
    x + 1
}

```