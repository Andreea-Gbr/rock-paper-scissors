# Rock, Paper, Scissors (Python)

A simple command-line implementation of the classic Rock, Paper, Scissors game written in Python.

The player competes against the computer in an interactive loop until choosing to exit.

---

## Features

- Play against the computer
- Random computer choice using Python’s `random` module
- Case-insensitive user input (e.g., "ROCK", "Rock", "rock" all work)
- Input validation for incorrect choices
- Continuous play mode
- Option to exit the game at any time

---

## How It Works

1. The program defines three possible choices:
   - rock
   - paper
   - scissors

2. The computer randomly selects one option each round using `random.choice()`.

3. The user is prompted to enter:
   - rock
   - paper
   - scissors
   - or "exit" to quit the game

4. The user input is converted to lowercase using `.lower()` to ensure case-insensitive comparison.

5. The program:
   - Validates user input
   - Compares choices
   - Determines the winner based on classic game rules
   - Displays the result

The game continues in a loop until the user types `exit`.

---

## Requirements

- Python 3.x

No external libraries are required.

---

## How to Run

From the project directory:

```bash
python rock_paper_scissors.py
```

Or (depending on your system):

```bash
python3 rock_paper_scissors.py
```

---

## Example Usage

```
Welcome to Rock, Paper, Scissors!
Choose rock, paper, or scissors (or 'exit'): rock
Computer chose: scissors
You win!
```

If invalid input is entered:

```
Invalid choice. Try again.
```

To exit:

```
Choose rock, paper, or scissors (or 'exit'): exit
Thanks for playing!
```

---

## Project Structure

Single-file implementation:

```
rock_paper_scissors.py
```

Main components:
- `options` list – contains valid choices
- `random.choice()` – generates computer selection
- `while True` loop – enables continuous gameplay
- Conditional logic – determines winner

---

## Optional Extensions

- Add score tracking (wins, losses, ties)
- Add best-of-three or best-of-five mode
- Add difficulty levels (computer strategy instead of purely random)
- Add a match history log (show last N rounds)
- Add a graphical user interface (GUI)
