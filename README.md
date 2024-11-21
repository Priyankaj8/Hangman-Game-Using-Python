# Hangman Game

A console-based **Hangman** game implemented in Python. The player tries to guess a randomly chosen word one letter at a time before running out of lives.

## Features
- Randomly selects a word from a predefined list.
- Tracks the player's guesses and displays progress visually using Hangman stages.
- Provides feedback on repeated guesses and incorrect guesses.
- Win or lose conditions based on the player's remaining lives and guessed letters.

## How It Works
1. A random word is selected from the `word_list`.
2. The player has 6 lives to guess the word.
3. The game provides:
   - Feedback if the guessed letter is correct.
   - A warning if the guessed letter has already been tried.
   - Updates to the word display and remaining lives after each guess.
4. The game ends when:
   - The player guesses the entire word correctly (*Win*).
   - The player runs out of lives (*Lose*).

## Getting Started

### Prerequisites
- Python 3.x installed on your system.
- The `hangman_words.py` file containing a list of words as `word_list`.
- The `hangman_stages.py` file containing Hangman ASCII art as `stages`.

## Example Gameplay

Below is an example of how the game might look when played in the console:

```text
_ _ _ _ _ _ 
*************************6/6 LIVES LEFT**********************
Guess a letter: a
______
Your guess a, that's not in the word! You lose a life

 +---+
 |   |
 O   |
     |
     |
     |
========

*************************5/6 LIVES LEFT**********************
Guess a letter: i
______
Your guess i, that's not in the word! You lose a life

 +---+
 |   |
 O   |
/    |
     |
     |
========

*************************4/6 LIVES LEFT**********************
Guess a letter: c
______
Your guess c, that's not in the word! You lose a life

 +---+
 |   |
 O   |
/|   |
     |
     |
========

*************************3/6 LIVES LEFT**********************
Guess a letter: u
___u__

 +---+
 |   |
 O   |
/|   |
     |
     |
========

*************************3/6 LIVES LEFT**********************
Guess a letter: g
__gu__

 +---+
 |   |
 O   |
/|   |
     |
     |
========

*************************3/6 LIVES LEFT**********************
Guess a letter: e
__gu__
Your guess e, that's not in the word! You lose a life

 +---+
 |   |
 O   |
/|\  |
     |
     |
========

*************************2/6 LIVES LEFT**********************
Guess a letter: i
__gu__
Your guess i, that's not in the word! You lose a life

 +---+
 |   |
 O   |
/|\  |
/    |
     |
========

*************************1/6 LIVES LEFT**********************
Guess a letter: n
__gu__
*************************It was yogurt! YOU LOSE!************************

 +---+
 |   |
 O   |
/|\  |
/ \  |
     |
========
