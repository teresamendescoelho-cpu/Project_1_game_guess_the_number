# 🎯 Project 1 — Number Guessing Game

A Python Number Guessing Game developed as the first project of the Ironhack Data Analytics Bootcamp.

The project was designed to apply fundamental Python programming concepts through the development of a fully playable interactive game.

The player must guess a randomly generated number between 1 and 100, with a maximum of 10 attempts. The game provides feedback after each guess and keeps track of the player's progress.

---

## 🎓 Project Purpose

This project was part of the "Quest: Build Your Game" project from the Ironhack Data Analytics Bootcamp.

The main purpose was to put Python fundamentals into practice by designing and developing a functional game from the initial idea through to a playable version.

The project focused on applying concepts such as:

- Functions
- Flow control
- Loops
- Lists
- Dictionaries
- Modules
- Input validation
- Error handling
- Documentation
- Game state management

The project also required the game to have clear rules, winning and losing conditions, and a complete gameplay loop.

---

## 🎮 Game Overview

The computer randomly generates a secret number between 1 and 100.

The player has up to 10 attempts to discover the secret number.

After every guess, the game provides feedback:

- 📈 Too high
- 📉 Too low
- 🎉 Correct

The game ends when the player guesses the secret number or uses all available attempts.

After the game ends, the player can choose whether to play again.

---

## 🕹️ How to Play

1. Start the game.
2. The computer generates a secret number between 1 and 100.
3. Enter your guess.
4. Receive feedback about your guess.
5. Check the number of remaining attempts.
6. Continue guessing until you win or run out of attempts.
7. Choose whether to play again.

Example gameplay:

🎯 NUMBER GUESSING GAME

I'm thinking of a number between 1 and 100.
You have 10 attempts.

Enter your guess: 70

📈 Too high!
Attempts remaining: 9

Enter your guess: 35

📉 Too low!
Attempts remaining: 8

Enter your guess: 52

🎉 Correct!
You won in 3 attempts!

Would you like to play again? (y/n):

---

## 🎯 Game Rules

- The secret number is randomly generated between 1 and 100.
- The player has a maximum of 10 attempts.
- Each guess must be between 1 and 100.
- The game provides feedback after each guess.
- Remaining attempts are displayed throughout the game.
- The player wins by guessing the secret number.
- The player loses after 10 incorrect attempts.
- The player can start a new game after finishing.

---

## 🛠️ Technologies & Tools

### Programming Language

Python

Python was used to develop the game logic, implement the game state, handle user input and control the gameplay.

### Development Environment

Jupyter Notebook / Google Colab

The project was developed and tested using Jupyter Notebook and Google Colab.

### Version Control

Git & GitHub

Git and GitHub are used to manage the project files, track development and document the final project.

### Main Python Concepts

- Functions
- Variables
- if / elif / else
- for loops
- while loops
- Lists
- Dictionaries
- Modules
- Random number generation
- Input validation
- try / except
- Error handling
- Documentation

---

## 🗃️ Data Structures

Although this is a game rather than a traditional data analytics project, data structures are an important part of the implementation.

### List

A list is used to store the guesses made by the player.

Example:

    guesses = [50, 25, 42]

This allows the game to keep a record of the player's guesses.

### Dictionary

A dictionary is used to store named information about the current game state and results.

Example:

    game_state = {
        "secret_number": 42,
        "attempts_used": 3,
        "remaining_attempts": 7,
        "guesses": [50, 25, 42],
        "won": True
    }

---

## 🔄 Game State

The game_state dictionary keeps track of the current status of the game.

It contains information such as:

- Secret number
- Attempts used
- Remaining attempts
- Player guesses
- Win status

The state is updated as the player progresses through the game.

---

## 🛡️ Input Validation & Error Handling

The game validates user input before processing a guess.

Examples of invalid input include:

- Text instead of a number
- Empty input
- Numbers below 1
- Numbers above 100

The program uses error handling to prevent invalid input from crashing the game.

Example message:

    Please enter a valid number between 1 and 100.

---

## 🔁 Play Again

After a game is completed, the player can choose to start a new game.

Example:

    Game over!

    Would you like to play again? (y/n):

Choosing y starts a new game with a new secret number and resets the attempts.

Choosing n ends the game.

---

## 📁 Repository Structure

The GitHub repository is organized to separate the game, supporting files, documentation and presentation.

    Project_1_game_guess_the_number/
    │
    ├── README.md
    ├── .gitignore
    │
    ├── main.ipynb
    │
    ├── game.py
    ├── utils.py
    │
    └── presentation/
        └── project-1-presentation.pptx

### File Description

| File / Folder | Purpose |
|---|---|
| README.md | Project documentation and instructions |
| .gitignore | Specifies files and folders that should not be tracked by Git |
| main.ipynb | Main Jupyter Notebook used to run and demonstrate the game |
| game.py | Main game logic and gameplay functions |
| utils.py | Helper and utility functions |
| presentation/ | Project presentation |
| project-1-presentation.pptx | Final project presentation |

---

## 🧩 Main Functions

The game is organized around functions with specific responsibilities.

### generate_secret_number()

Generates the random secret number.

### get_player_guess()

Gets and validates the player's input.

### check_guess()

Compares the player's guess with the secret number.

### update_game_state()

Updates the game state after each attempt.

### check_game_over()

Checks whether the player has won or lost.

### play_again()

Handles the option to start another game.

### number_guessing_game()

Controls the overall gameplay.

---

## 🧪 Testing

The game is tested using different scenarios to make sure it behaves correctly.

### Gameplay

- Correct guess
- Guess too high
- Guess too low
- Win on the first attempt
- Win on the final attempt
- Lose after 10 attempts

### Input Validation

- Text input
- Empty input
- Number below 1
- Number above 100

### Play Again

- Select y
- Select n
- Invalid response

---

## 🚀 Possible Future Improvements

Possible extensions include:

- Difficulty levels
- High-score system
- Win-rate statistics
- Number of games played
- Best score
- Different number ranges
- Additional game modes
- Improved user interface

---

## 🎓 Bootcamp Context

School: Ironhack

Program: Data Analytics Bootcamp

Project: Project 1 — Quest: Build Your Game

Game: Number Guessing Game

Author: Teresa Mendes Coelho

The project was developed as an opportunity to apply Python fundamentals through a practical, interactive programming challenge.

---

## 👩‍💻 Author

Teresa Mendes Coelho

Data Analytics | Python | SQL | Data Visualization

GitHub: https://github.com/teresamendescoelho-cpu
