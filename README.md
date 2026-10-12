# Rock Paper Scissors Game

A simple command-line Rock Paper Scissors game where you play against the computer. Built in Python as a learning project to practice game logic and user input.

## Features

- **Play Against Computer**: The computer randomly selects rock, paper, or scissors
- **Input Validation**: Only accepts valid choices (rock, paper, scissors)
- **Instant Feedback**: Shows both player and computer choices, then displays the result
- **Play Multiple Rounds**: Option to play again without restarting the program
- **Game Rules**: Standard rock-paper-scissors rules
  - Rock beats Scissors
  - Scissors beats Paper
  - Paper beats Rock
  - Same choice = Tie

## How to Use

1. **Run the program**:
   ```bash
   python rock_paper_scissors.py
   ```

2. **Enter your choice**:
   ```
   Enter a choice (rock, paper, or scissors): rock
   ```

3. **View results**:
   ```
   Player: rock
   Computer: scissors
   You win!
   ```

4. **Play again**:
   ```
   Do you want to play again? (y/n): y
   ```

## Requirements

- Python 3.x
- Built-in `random` module (no external libraries needed)

## How It Works

| Component | Explanation |
|-----------|-------------|
| **Input Validation** | Loops until user enters a valid choice |
| **random.choice()** | Randomly picks rock, paper, or scissors for computer |
| **Game Logic** | Uses if/elif statements to determine winner |
| **Play Again Loop** | Allows multiple games in one session |

## Code Breakdown

```python
# Generate random computer choice
computer = random.choice(options)

# Validate player input
while player not in options:
    player = input("Enter a choice (rock, paper, or scissors): ")

# Determine winner using game rules
if player == computer:
    print("It's a tie!")
elif player == "rock" and computer == "scissors":
    print("You win!")
# ... more conditions ...
else:
    print("You lose!")
```

## Learning Concepts

This project teaches:
- ✅ Using the `random` module
- ✅ While loops for input validation
- ✅ Nested if/elif/else statements
- ✅ String comparison
- ✅ User input handling
- ✅ Boolean logic with `running` flag

## Possible Improvements

- Add score tracking (wins/losses/ties)
- Display game statistics after quitting
- Add difficulty levels (hard AI strategy)
- GUI interface using tkinter
- Add more game modes
- Store game history to a file


