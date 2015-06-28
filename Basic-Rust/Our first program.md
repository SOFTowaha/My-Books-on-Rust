###Our first program

Let’s get started by showing a welcome message to our players. Open your favorite text editor (like notepad or gedit) 
for a new file and type in the following code:

```rust
fn main() {
    println!(""Hello Bangladesh!"");
}
```

•	Save the file as 
```rust
welcome.rs
```
rs is the standard extension of Rust code files. Source file names containing more than one word use an 
underscore _ as separator, for example: start_game.rs

*	Then compile it to native code on the command line with:       
```rust
	rustc welcome.rs 
```

This produces an executable program welcome.exe on Windows or welcome on Linux. 

*	Run this program with: welcome or ./welcome to get the output:

Hello Bangladesh!
The output executable gets its name from the source file. If you want to give the executable another name, 
like start, compile it with option -o output_name:
```rust
		rustc welcome.rs -o start
```
Compiling and running are separate consecutive steps, contrary to dynamic languages like Ruby or Python where 
these are performed in one step.
Let’s explain the code a bit. If you have already worked in a C/Java/C# like environment this code will seem 
quite familiar. As in most languages execution of code starts in a main() function, which is mandatory in an 
executable program. 

In a larger project with many source files the file containing the main() function would be called main.rs by 
convention.
We see that main() is a function declaration because it is preceded by the keyword fn, short and elegant like 
most Rust keywords. The () after main denote the parameter list, which is empty here. The function’'s code 
is placed in a code block, surrounded by curly braces { }, where the opening brace is put by convention on 
the same line as the function declaration but separated by one space. The closing brace appears after the code, 
right beneath fn. 
Our program has only one line, which is indented by 4 spaces to improve readability. This line prints the string 
“"Hello Bangladesh!”". Rust recognizes this as a string because it is surrounded by double quotes " ". 

This string was given as argument to the println! macro (the ! indicates it is a macro and not a function). 
The code line ends in a semicolon ; as most, but not all, code lines in Rust do (see next chapter).

*Exercises:*   
* 1) Write, compile and execute a Rust program name.rs that prints out your name.
* 2) What is the smallest possible program in Rust?
* 
Here is an alternative version that produces exactly the same output and illustrates how to use a function from an external library or crate as Rust calls them; in this case the println function comes from the module io in the crate std, which is the standard library of Rust:

```rust
use std::io;

fn main() {
		io::println(""Welcome to the Game!"");	
}
```


The println! macro is preferred over the simple println function, because it has some nice formatting capabilities and at the same time checks when compiling whether the type of variables is correct for the applied formatting .
