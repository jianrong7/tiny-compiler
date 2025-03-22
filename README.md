# tiny-compiler

Use Python to implement our own programming language to compile to C code.

Let's call this language "Tiny". It will be a dialect of BASIC.

This is done based on this [tutorial](https://austinhenley.com/blog/teenytinycompiler1.html).

## Tiny Language Features

- Numerical variables
- Basic arithmetic
- If statements
- While loops
- Print text and numbers
- Input numbers
- Labels and goto
- Comments

**Notable features not included:**

- Functions
- Arrays
- File IO
- Else statement

## Components of a compiler

Lexer --> Parser --> Emitter

### Lexer

- Receives input source code
- Breaks it down into tokens

### Parser

- Paarse tokens to make sure they are in an order that is allowed in Tiny

### Emitter

- Emit the C code that Tiny will translate to
