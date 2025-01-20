# Guessing Game Flowchart

The following flowchart represents the logic of a simple guessing game. The game generates a random number between 1 and 100, and the player must guess the correct number. Here is a step-by-step breakdown of the process:

1. **Start the Game**:  
   The program begins by generating a random number between 1 and 100.

2. **Prompt for User Input**:  
   The player is prompted to enter a guess.

3. **Validate the Input**:  
   - If the input is **not a valid number**, the program displays an error message ("Enter a Valid Number") and prompts the user to guess again.
   - If the input **is valid**, the program proceeds to check if the number is within the valid range.

4. **Check if the Guess Is Within Range**:  
   - If the guess is **out of range** (not between 1 and 100), the program displays an error message ("Guess Out of Range") and prompts the user to guess again.
   - If the guess is **within range**, the program checks if it matches the randomly generated number.

5. **Compare the Guess**:  
   - If the guess is **correct**, the program displays a success message ("Correct! You Win") and ends the game.
   - If the guess is **incorrect**, the program determines if it is too high or too low.

6. **Provide Feedback**:  
   - If the guess is **too high**, the program displays a hint ("Too High! Try Again") and prompts the user for another guess.
   - If the guess is **too low**, the program displays a hint ("Too Low! Try Again") and prompts the user for another guess.

7. **End the Game**:  
   The game ends when the correct number is guessed.

This diagram and explanation outline the logical flow of the guessing game, ensuring clarity and ease of understanding for developers and users.
