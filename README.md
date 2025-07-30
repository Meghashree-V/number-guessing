# Number Guessing Game using Rust

This is a simple command-line number guessing game implemented in Rust. The game demonstrates fundamental Rust concepts such as variables, input/output, loops, conditionals, external crates, and random number generation.

## How to Play
- The program randomly selects a number between 1 and 100.
- You are prompted to guess the number.
- After each guess, the program will tell you if your guess is too low, too high, or correct.
- If you guess the correct number, the game congratulates you and ends.

## How It Works
1. The program prints a welcome message and instructions.
2. It generates a random number using `rand::thread_rng().gen_range(1..=100)`.
3. It enters a loop where it prompts the user for a guess:
    - If the input is not a valid number, it asks again.
    - If the guess is too low or too high, it gives feedback.
    - If the guess is correct, it congratulates you and exits.

## Running the Game
Make sure you have Rust and Cargo installed.

Open a terminal in this directory and run:

```bash
cargo run
```

## Example Output
```
Guess the number!
I'm thinking of a number between 1 and 100.
Please input your guess.
50
You guessed: 50
Too high!
Please input your guess.
25
You guessed: 25
Too low!
Please input your guess.
37
You guessed: 37
Congratulations! You guessed the number 37 correctly!
```

## Concepts Demonstrated
- `use` for bringing libraries into scope
- `rand` crate for random number generation
- `io::stdin()` for user input
- `println!` macro for output
- `loop` and control flow (`if`, `else if`, `else`)
- Pattern matching with `match` for input parsing

---
Inspired by the Rust "Guessing Game" project from The Rust Programming Language book.
