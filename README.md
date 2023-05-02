# rust-solutions

# Week 10 Mini project

## Guessing game

```
cd guessing_game
cargo run
```

* This function first prints the welcome message for the number guessing game and then uses the thread_rng() function in rand crate to generate a random number secret_number, an integer in the range 1 to 100.

* I am using a loop to repeatedly prompt the user for the guess number. The stdin function in the io standard library is then used to get the string entered by the user and store it in a variable of type String

* The code uses the match statement to convert the user input string to a number of type u32. If the conversion succeeds, the number is stored in the guess variable. If the conversion fails, the code continues to prompt the user for input.

* Finally, the code compares the number guessed by the user with secret_number and outputs the corresponding message according to the result. If the user guesses correctly, the code prints the message "You win!" and uses the break keyword to end the loop and the program. If the user guesses a number smaller than secret_number, the message "Too small!" will be printed. If the user guesses a number larger than secret_number, the message "Too big!" will be printed. This process will continue to loop until the user guesses correctly.
