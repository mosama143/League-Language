# LeagueLang

**LeagueLang** is a fantasy-style programming language implemented in Python.  
It is inspired by game-like commands such as `SUMMON`, `RECALL`, `ULTIMATE`, and others.  
The project currently includes a **tokenizer (lexer)** and will be expanded with a **parser**, interpreter, and more.

---

## Features

- Tokenizes game-inspired commands and categorizes them into:
  - Program Structure (`SUMMON`, `RECALL`, `USE`)
  - Variables (`BUILD`)
  - Input/Output (`SAY`, `LISTEN`)
  - Control Flow (`CHECK`, `MISS`, `FARM`, `FF15`)
  - Functions (`ULTIMATE`, `CALL`, `BASE`)
- Easily extendable for new commands or syntax rules.
- Written in Python using `re` and `dataclasses` for clean and structured code.

---

## Example Usage

```python
USE DEMACIA
SUMMON GAME

BUILD CHAMPION name = "Garen"
BUILD POWER gold = 0
SAY "Welcome, " + name + "!"

CHECK (gold >= 1000) {
    SAY "You're rich!"
}
MISS {
    SAY "Keep FARMING!"
}

ULTIMATE SpinToWin() {
    SAY "SPIN TO WIN!"
    BASE
}

CALL SpinToWin
RECALL BASE
