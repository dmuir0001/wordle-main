# Wordle Clone -- README

## Overview

This project is a JavaScript implementation of a Wordle clone for
**CS390 Mini Project 1**. The game selects a random five-letter word,
and players have six attempts to guess it, receiving feedback through
colored tiles and an on-screen keyboard.

## Design & Implementation

-   **initializeGame():** Resets state, selects a random word, clears
    the board, and hides modals.\
-   **handleKeyPress():** Processes letter, ENTER, and BACKSPACE keys as well as
    updating tiles and guesses.\
-   **submitGuess():** Validates guesses, checks letters, updates
    tiles/keyboard, and calls `updateGameState()`.\
-   **checkLetter():** Returns `correct`, `present`, or `absent` for
    each letter.\
-   **updateGameState():** Ends game on win/loss and shows results.

### Advanced Features

-   **updateKeyboardColors():** Updates keyboard with color indicator
    (green \> yellow \> gray).\
-   **processRowReveal():** Triggers celebration if a row is completely
    correct.\
-   **showEndGameModal():** Displays win/lose messages and updates
    statistics.\
-   **validateInput():** Prevents invalid actions and ensures input
    rules are followed.
