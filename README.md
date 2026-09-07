# 🎯 Project 1 — Number Guessing Game

A Python **Number Guessing Game** developed as the first project of the
**Ironhack Data Analytics Bootcamp**.

The project applies fundamental Python programming concepts through the
development of a fully playable and interactive game.

The player tries to guess a randomly generated number within the
selected difficulty level. The original Ironhack requirement is
preserved in **Classic mode: 1–100 with a maximum of 10 attempts**.

------------------------------------------------------------------------

## 🎓 Project Purpose

This project was part of the **“Quest: Build Your Game”** project from
the Ironhack Data Analytics Bootcamp.

The main purpose was to put Python fundamentals into practice by
designing and developing a functional game from the initial idea through
to a complete playable version.

The project focuses on:

- Functions
- Flow control
- `for` and `while` loops
- Lists
- Dictionaries
- Game state management
- Modules and imports
- Input validation
- Error handling
- Comments and docstrings
- Random number generation

------------------------------------------------------------------------

## 🎮 Game Overview

The computer randomly generates a secret number.

The player selects one of three difficulty levels:

| Difficulty | Number Range | Attempts |
|------------|-------------:|---------:|
| 🟢 Easy    |         1–50 |       10 |
| 🔵 Classic |        1–100 |       10 |
| 🔴 Hard    |        1–100 |        8 |

**Classic mode** follows the original Ironhack project requirement: the
player has a maximum of **10 attempts to guess a number between 1 and
100**.

After every valid guess, the game provides feedback:

- 📈 **Too high**
- 📉 **Too low**
- 🎉 **Correct**

The game ends when the player guesses the secret number or uses all
available attempts.

After each completed game, the player can choose whether to play again.

------------------------------------------------------------------------

## 🕹️ How to Play

1.  Start the game.
2.  Choose a difficulty level.
3.  The computer generates a random secret number within the selected
    range.
4.  Enter your guess.
5.  Receive feedback about your guess.
6.  Check the number of remaining attempts.
7.  Continue guessing until you win or run out of attempts.
8.  Choose whether to play again.

------------------------------------------------------------------------

## 🎯 Game Rules

- The secret number is generated randomly.
- Easy mode uses numbers from **1 to 50** with 10 attempts.
- Classic mode uses numbers from **1 to 100** with 10 attempts.
- Hard mode uses numbers from **1 to 100** with 8 attempts.
- Each guess must be within the selected number range.
- Invalid input does not count as an attempt.
- The game provides feedback after every valid guess.
- Remaining attempts are displayed after every valid guess.
- The player wins by guessing the secret number.
- The player loses when all available attempts are used without guessing
  correctly.
- The player can start a new game after finishing.

------------------------------------------------------------------------

## 🛠️ Technologies & Tools

### Programming Language

**Python**

### Development Environment

**Jupyter Notebook / Google Colab**

### Version Control

**Git & GitHub**

### Main Python Concepts

- Variables
- Functions
- `if / elif / else`
- `for` loops
- `while` loops
- Lists
- Dictionaries
- Modules
- Imports
- Random number generation
- Input validation
- `try / except`
- Error handling
- Comments
- Docstrings

------------------------------------------------------------------------

## 🗃️ Data Structures

Although this is a game rather than a traditional data analytics
project, data structures are an important part of the implementation.

### List

A list stores the guesses made by the player.

Example:

``` python
guesses = [50, 25, 42]
```

### Dictionary

A dictionary stores named information about the current game state and
results.

Example:

``` python
game_state = {
    "secret_number": 42,
    "difficulty": "Classic",
    "attempts_used": 3,
    "remaining_attempts": 7,
    "guesses": [50, 25, 42],
    "won": True
}
```

------------------------------------------------------------------------

## 🔄 Game State

The `game_state` dictionary keeps track of the current status of each
game.

It contains:

- Secret number
- Difficulty
- Attempts used
- Remaining attempts
- Player guesses
- Win status

The game state is updated after every valid guess.

------------------------------------------------------------------------

## 🛡️ Input Validation & Error Handling

The game validates user input before processing a guess.

Invalid input includes:

- Text instead of a number
- Empty input
- Numbers below the selected minimum
- Numbers above the selected maximum
- Invalid difficulty choices
- Invalid Play Again responses

The program uses `try / except` to prevent invalid numeric input from
crashing the game.

Invalid guesses outside the selected range are rejected and do not
consume an attempt.

------------------------------------------------------------------------

## ⭐ Additional Features

In addition to the original game requirements, the project includes:

### Difficulty Levels

- **Easy:** 1–50 with 10 attempts
- **Classic:** 1–100 with 10 attempts
- **Hard:** 1–100 with 8 attempts

### Play Again

After completing a game, the player can start another game. Each new
game generates a new secret number and resets the game state.

### Session Statistics

At the end of the session, the program displays:

- Games played
- Games won
- Overall win rate

### Improved User Interface

The game includes formatted sections, clear instructions, difficulty
information, attempt tracking, and previous guesses.

------------------------------------------------------------------------

## 📁 Repository Structure

``` text
Project_1_game_guess_the_number/
│
├── README.md
├── .gitignore
├── number_guessing_game.ipynb
│
└── presentation/
    └── project-1-presentation.pptx
```

### File Description

| File / Folder                 | Purpose                                                       |
|-------------------------------|---------------------------------------------------------------|
| `README.md`                   | Project documentation and instructions                        |
| `.gitignore`                  | Specifies files and folders that should not be tracked by Git |
| `number_guessing_game.ipynb`  | Main Jupyter Notebook containing the game                     |
| `presentation/`               | Project presentation                                          |
| `project-1-presentation.pptx` | Final project presentation                                    |

------------------------------------------------------------------------

## 🧩 Main Functions

The game is organized into functions with specific responsibilities.

- **`choose_difficulty()`** — selects the difficulty and its number
  range/attempt limit.
- **`get_player_guess()`** — gets and validates the player’s input.
- **`check_guess()`** — compares the guess with the secret number.
- **`update_game_state()`** — updates the game state after each valid
  guess.
- **`display_game_status()`** — displays attempts and previous guesses.
- **`check_game_over()`** — checks whether the game has reached a win or
  lose condition.
- **`play_one_game()`** — controls one complete game.
- **`play_again()`** — handles starting another game.
- **`number_guessing_game()`** — controls the complete session and
  calculates statistics.

------------------------------------------------------------------------

## 🧪 Testing

The game was tested with different gameplay and input scenarios.

### Gameplay Tests

- Correct guess
- Guess too high
- Guess too low
- Win on the first attempt
- Win on the final available attempt
- Lose after all available attempts
- Repeated guesses
- Multiple games

### Input Validation Tests

- Text instead of a number
- Empty input
- Number below the selected range
- Number above the selected range
- Invalid difficulty selection
- Invalid Play Again response

### Difficulty Tests

- Easy: 1–50 / 10 attempts
- Classic: 1–100 / 10 attempts
- Hard: 1–100 / 8 attempts

------------------------------------------------------------------------

## 🎓 Bootcamp Context

**School:** Ironhack

**Program:** Data Analytics Bootcamp

**Project:** Project 1 — Quest: Build Your Game

**Game:** Number Guessing Game

**Author:** Teresa Mendes Coelho

The project was developed as an opportunity to apply Python fundamentals
through a practical, interactive programming challenge.

------------------------------------------------------------------------

## 📚 Learning Outcomes

Through this project, I practiced:

- Structuring a Python program using functions
- Managing game state with dictionaries
- Working with lists to store dynamic information
- Using loops and conditional statements
- Handling user input and errors
- Using Python modules
- Writing documentation with docstrings
- Testing different gameplay scenarios
- Organizing a project for GitHub
- Turning a basic programming exercise into a complete interactive
  application

------------------------------------------------------------------------

## 👩‍💻 Author

**Teresa Mendes Coelho**

Data Analytics \| Python \| SQL \| Data Visualization

GitHub: https://github.com/teresamendescoelho-cpu
