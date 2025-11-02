# ArcaneLang

ArcaneLang is a fantasy-style programming language implemented in Python. 
It currently includes a tokenizer (lexer) and will be expanded with a parser, interpreter, and more.

## Features
- Tokenizes game-inspired commands like SUMMON, RECALL, ULTIMATE.
- Categorizes tokens into program structure, variables, I/O, and control flow.
- Designed to be extendable for building a full programming language.

## Example
```python
USE DEMACIA
SUMMON GAME
BUILD CHAMPION name = "Garen"
SAY "Welcome, " + name + "!"
