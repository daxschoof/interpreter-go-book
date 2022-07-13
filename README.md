# Monkey Interpreter
Building a tree-walking interpreter using "Writing an Interpreter in Go"

## Chapter 1 - Lexers
Source Code --> Tokens --> Abstract Syntax Tree

A lexer parses source code into tokens through a process called "lexical analysis" or "lexing". The output is a series of constants predefined by the language. = may turn into EQUALS or an integer, whereas a non-key character like 9.5 may turn into DECIMAL(9.5).

Lexers use switches on characters to create tokens based on whatever it reads. If it reads a non-key character, it reads the rest of the word/number/else and assigns it as an identifier, number, or illegal token.
