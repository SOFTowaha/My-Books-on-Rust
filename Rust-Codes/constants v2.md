```rust
static MAXHEALTH: i32 = 300;
static GAMENAME: &'static str = "Bitch Please";

fn main() {
	println!("The Game you are going to playg is called {}.", GAMENAME);
	println!("You start with {} health points.", MAXHEALTH);
	println!("In the Game {0} you start with {1} % health, yes you read it correctly: {1} points!", 
		GAMENAME, MAXHEALTH);
	println!("You have {points} % health", points=70);

	// formatting:
	println!("MAXHEALTH is {:x} in hexadecimal", MAXHEALTH);
	println!("MAXHEALTH is {:b} in binary", MAXHEALTH);
}

```
