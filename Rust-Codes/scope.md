```rust
fn main() {
	let outer = 42;
    { // start code block
        // This variable only exists in this block
        let inner = 3.14159;
        println!("block variable: {}", inner);
        let outer = 99; // shadows the first outer variable
        println!("block variable outer: {}", outer);
    } // end of code block
    // println!("out of block: {}", inner);  // error: unresolved name inner
    println!("outer variable: {}", outer);
}

```
