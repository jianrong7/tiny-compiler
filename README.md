# tiny-compiler

I was sad that I never had the chance to take the compiler class during college. I am no longer sad after this.

However, this implementation is quite simple, not even requiring an AST. I will work on something more ambitious soon.

Use Python to implement our own programming language to compile to C code.

Let's call this language "Tiny". It will be a dialect of BASIC.

This is done based on this [tutorial](https://austinhenley.com/blog/teenytinycompiler1.html).

## How to use?

Run `bash build.sh ./examples/average.tiny` to compile the Tiny code to C code.
The corresponding C file and executable should appear. Now you can run them using `./average` and also check out the compiled C code in `average.c`.

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
