
# 📘 Assignment: Hangman Game Challenge

## 🎯 Objective

Build the classic Hangman word-guessing game using Python strings, loops, conditionals, and user input. Players will guess letters to reveal a hidden word before running out of attempts.

## 📝 Tasks

### 🛠️ Core Game Mechanics

#### Description
Implement the core functionality of the Hangman game, including word selection, tracking guesses, and managing game state.

#### Requirements
Completed program should:

- Randomly select words from a predefined list
- Accept letter guesses and show current progress (_ _ _ format)
- Track incorrect guesses remaining
- Check if guessed letters are in the hidden word

### 🛠️ Game Flow & User Experience

#### Description
Manage the game loop and provide clear feedback to the player throughout the game.

#### Requirements
Completed program should:

- End the game when the word is guessed or attempts are exhausted
- Display clear win/lose messages
- Show the number of attempts remaining after each guess
- Allow the player to play multiple rounds if desired

#### Example Output
```
Welcome to Hangman!
_ _ _ _ _
Guesses remaining: 6
Guess a letter: e
_ _ _ e _
Guesses remaining: 6
Guess a letter: a
_ _ _ e a
Guesses remaining: 6
Guess a letter: x
_ _ _ e a
Guesses remaining: 5
...
_ o _ e a
You won! The word was: homeà
Play again? (yes/no): no
Thanks for playing!
```
